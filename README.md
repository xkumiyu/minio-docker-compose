# MinIO Docker Compose Examples

[minio](https://github.com/minio/minio)

## No SSL

```sh
cd no-ssl
```

create `.env` file as follow:

```ini
# root user
ROOT_USER=minio
ROOT_PASSWORD=password

# non-root user
ACCESS_KEY_ID=AKIAIOSFODNN7EXAMPLE
SECRET_ACCESS_KEY=wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY
USER_POLICY=readwrite

# bucket
BUCKET_NAME=default
```

## SSL

```sh
cd ssl
```

add the following to `.env` file of non-ssl:

```ini
MINIO_HOST=example.com
CONSOLE_HOST=console.example.com
```
