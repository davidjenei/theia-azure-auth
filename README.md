```
az ad sp create --id theia -o yaml
cp env .env # Set environment variables
docker-compose config
./init-letsencrypt.sh
docker-compose up -d
```