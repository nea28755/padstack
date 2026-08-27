# padstack

Minimal notes REST API built with Flask

Built for my own use; public in case it helps someone.

## Installation

```bash
pip install -r requirements.txt
flask --app app run --debug
```

## Examples

```bash
curl -X POST localhost:5000/notes \
  -H 'content-type: application/json' \
  -d '{"title": "first", "body": "hello"}'
```

## Features

- SQLite storage via sqlite3 stdlib
- CRUD endpoints for notes
- pytest coverage for the happy paths
- Request validation and consistent error shape

## Project structure

```text
├── docs/
│   ├── development.md
│   ├── roadmap.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   ├── test_api.py
│   └── test_smoke.py
├── .editorconfig
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
├── Makefile
├── SECURITY.md
├── app.py
└── requirements.txt
```

## License

MIT licensed, see LICENSE.
