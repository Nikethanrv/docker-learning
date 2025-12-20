### Installing Postgres container with ny_taxi DB 
docker run -it --rm \
-e POSTGRES_USER=root \
-e POSTGRES_PASSWORD=root \
-e POSTGRES_DB=ny_taxi \
-v ny_taxi_postgres_data:/var/lib/postgresql \
-p 5432:5432 \
postgres:18

### Connecting to Postgres
TZ=UTC uv run pgcli -h localhost -p 5432 -u root -d ny_t
axi

### Opening Jupyter Notebook
uv add --dev jupyter
uv run jupyter notebook