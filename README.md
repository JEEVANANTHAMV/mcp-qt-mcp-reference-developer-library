# Qt MCP (Reference / Developer Library)

> Ships the signal-slot/qtmcp C++ library source (QtMcp::Server / QtMcp::Client) for Qt developers building their own MCP-speaking application. This is NOT a turnkey tool — it has no automation capabilities of its own.

The bundle zip (**30.2 MB**) is stored in this repository at **`4daca5d6-e883-41ed-a903-edaff5435715.zip`**.

This repository is part of the **Forjinn-Desk** MCP bundle collection. An MCP bundle is a self-contained server that a host application launches and communicates with over the MCP (Model Context Protocol) protocol.

## Repo metadata

| Field | Value |
| --- | --- |
| Registry ID | `4daca5d6-e883-41ed-a903-edaff5435715` |
| Status in registry | inactive |
| Bundle size | 30.2 MB |
| Distribution | committed to this repo |

## Environment variables

| Variable | Value / note |
| --- | --- |
| _(none)_ | _no required environment variables_ |

## MCP launch configuration

The host replaces `__INSTALL_DIR__` (install dir) and `__PYTHON__` (bundled Python) at runtime.

```json
{
  "command": "__PYTHON__",
  "args": [
    "server.py"
  ]
}
```

## Setup / usage notes

This bundle is reference material, not a usable tool. It requires Qt 6.8+, CMake 3.16+, and a C++20 compiler (none bundled) to actually build anything from the source. Its 3 tools only explain the library and let an agent browse the source — they do not control any application.


## Install / usage

1. Get the bundle:
   - download `4daca5d6-e883-41ed-a903-edaff5435715.zip` from this repo (Code → Download ZIP, or `git clone`).
2. Extract to your target installation directory (config paths expect contents at the install-dir root).
3. Set the environment variables listed above.
4. Launch using the MCP config JSON (or let a host client manage it automatically).

> Bundles may include vendored runtimes (bundled Python, Node, or native executables). Builds are Windows x64.
