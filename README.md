Deprecated: this module will not be used with Centrifuge >= 0.8.0

Centrifuge PostgreSQL structure backend
=======================================

Install:

```bash
pip install centrifuge-postgresql
```

If you get exception like:

```bash
Error: pg_config executable not found.
```

Then you don't have `libpq-dev` package installed on your machine. For example, for Debian:

```bash
sudo apt-get install libpq-dev
```

Or for Red Hat:

```bash
yum install postgresql-devel
```

When installed - enable it when launching  Centrifuge:

```javascript
CENTRIFUGE_STORAGE=centrifuge_postgresql.Storage centrifuge
```

inspect available options:

```javascript
CENTRIFUGE_STORAGE=centrifuge_postgresql.Storage centrifuge --help
```
