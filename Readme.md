## Для изменения статического файла в существующем образе nginx необходимо выполнить следующие команды

1. создать новый образ, используя Dockerfile
docker run -d --name=(name_of_your_image)  -p (your_host):80 -v (path_to_your_static_file):/usr/share/nginx/html nginx
2. Запустить хост
curl localhost:(your_host)/
