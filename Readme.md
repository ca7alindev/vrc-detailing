# LOCAL DEVELOPMENT
docker compose --file docker-compose.yml up --abort-on-container-exit

# LIVE DEVELOPMENT
ngrok http --domain=joint-snake-willingly.ngrok-free.app 8080

# DB DUMP
docker exec detailing-db mysqldump -u root -pca7alindev wordpress_db > init-db/install_db.sql