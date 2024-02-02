delete database
dotnet ef database drop -s API -p Persistence

reseed databaase
dotnet watch --no-hot-reload

add postgres to docker
docker run --name dev -e POSTGRES_USER=admin -e POSTGRES_PASSWORD=secret -p 5432:5432 -d postgres:latest