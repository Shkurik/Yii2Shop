1. Generate SSL certificates

    ```sh
    source .env && sudo docker run --rm -v $(pwd)/etc/ssl:/certificates -e "SERVER=$NGINX_HOST" jacoelho/generate-certificate
    ```
2. Start && stop the application :
    ```sh
    sudo docker-compose up -d
    sudo docker-compose down -v
    ```