## PostgreSQL Docker Setup

Run the following command to start a PostgreSQL container:

```bash
docker run --name postgres-container \
  -e POSTGRES_USER=postgres \
  -e POSTGRES_PASSWORD=0000 \
  -e POSTGRES_DB=spring_security \
  -e TZ=Asia/Kolkata \
  -e PGTZ=Asia/Kolkata \
  -p 5432:5432 \
  -v postgres_data:/var/lib/postgresql/data \
  -d postgres:15