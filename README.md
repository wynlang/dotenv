# dotenv — Official Wyn Package

Load `.env` files into HashMaps. Pure Wyn, no dependencies.

## Install

```bash
wyn pkg install github.com/wynlang/dotenv
```

## Usage

```wyn
var env = Dotenv_load(".env")
var db_host = env.get("DB_HOST")
var api_key = env.get("API_KEY")
```

`.env` file:
```
DB_HOST=localhost
DB_PORT=5432
API_KEY="secret123"
# This is a comment
DEBUG=true
```

## Test

```bash
wyn run tests/test_dotenv.wyn
```
