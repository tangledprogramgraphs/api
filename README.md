<div align="center">
<h3 align="center">Tangled Program Graphs API</h3>

  <p align="center">
    API for managing and interacting with Tangled Program Graph experiments.
  </p>
</div>

## Table of Contents

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#key-features">Key Features</a></li>
      </ul>
    </li>
    <li><a href="#built-with">Built With</a></li>
    <li><a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

## About The Project

This project provides a FastAPI-based API for managing and interacting with Tangled Program Graph (TPG) experiments. It allows users to evolve TPG agents within specified environments and replay existing experiments using a given seed. The API also includes WebSocket endpoints for real-time communication and signaling between clients.

### Key Features

- **Evolve Experiments:** Initiate TPG evolution within a specified environment. The API returns the seed and PID of the new experiment.
- **Replay Experiments:** Replay a TPG experiment using a specific environment and seed.
- **WebSocket Signaling:** Establish real-time communication channels between clients for signaling purposes. This is particularly useful for interactive experiments or demonstrations.
- **CORS Support:** Configured to allow requests from `http://localhost:8080` and `http://127.0.0.1:8080`, enabling local development and testing.

## Built With

- [FastAPI](https://fastapi.tiangolo.com/) - A modern, fast (high-performance), web framework for building APIs with Python 3.7+
- [uvicorn](https://www.uvicorn.org/) - ASGI server for running the FastAPI application.
- [pydantic](https://docs.pydantic.dev/) - Data validation and settings management using Python type annotations.
- [uv](https://github.com/astral-sh/uv) - Fast Python package installer and resolver.

## Getting Started

To get a local copy up and running, follow these steps.

### Prerequisites

- Python 3.12 or higher

### Installation

1.  Clone the repository

```sh
git clone https://github.com/tangledprogramgraphs/api.git
```

2.  Navigate to the project directory

```sh
cd api
```

3.  Install the dependencies using `uv`.

```sh
uv sync
```

4.  Running the API

```sh
uv run fastapi dev
```
