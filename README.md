Centrifuge PostgreSQL structure backend
=======================================

Install:

```bash
pip install centrifuge-postgresql
```

Enable in Centrifuge configuration file:

```javascript
{
    "structure": {
        "class": "centrifuge_postgresql.Storage",
        "settings": {
            "host": "localhost",
            "port": 5432,
            "name": "centrifuge",
            "password": "",
            "user": "postgres",
            "pool_size": 10
        }
    }
}
```

or

```javascript
{
    "structure": {
        "class": "centrifuge_postgresql.Storage",
        "settings": {
            "host": "localhost",
            "port": 5432,
            "name": "centrifuge",
            "password": "",
            "user": "postgres",
            "pool_size": 10
        }
    }
}
```

You can also specify PostgreSQL connection params as database url:

```javascript
{
    "structure": {
        "class": "centrifuge_postgresql.Storage",
        "settings": {
            "url": "postgres://user:pass@host:port/dbname"
        }
    }
}
```

Or specify an OS environment variable that holds value of the PostgreSQL connection url

```javascript
{
    "structure": {
        "storage": "centrifuge_postgresql.Storage",
        "settings": {
            "url": "$DATABASE_URL"
        }
    }
}

```