> **Fork of [Rikhil-Nell/MemoryWeave](https://github.com/Rikhil-Nell/MemoryWeave).** The fork keeps the upstream project history.

# MemoryWeave

A Python API that accepts a video and prompt, detects relevant objects, and stores a generated timeline. The code uses FastAPI, YOLO tracking, Pydantic AI, and Supabase.

## Current code

- Authenticated routes accept video uploads and return saved timelines.
- YOLO tracking records objects that match the submitted prompt.
- A Pydantic AI agent writes a first-person summary from the detected objects.
- Supabase calls store timeline records and frame metadata.

## Setup status

`pyproject.toml` requires Python 3.12 or newer and `uv.lock` records the dependency set. The checked-in `.sample.env` lists only the two Supabase values. `app/core/load_api.py` also requires provider settings that the sample does not list, so the repository does not yet give a complete local setup.
