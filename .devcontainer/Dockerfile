FROM ghcr.io/astral-sh/uv:0.12.17 AS uv
FROM mcr.microsoft.com/devcontainers/python:1-3.13-bookworm

COPY --from=uv /uv /uvx /usr/local/bin/

ENV UV_LINK_MODE=copy \
    PYTHONUNBUFFERED=1 \
    PATH="/workspaces/web-svc/.venv/bin:${PATH}"

USER vscode
