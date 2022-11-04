# cloud-computing-test-vm

ssh -i lab1 ronan-s@40.81.130.17

eval "$(ssh-agent -s)"

ssh-add labone

docker run -dp 80:3000 getting-started

http://40.81.130.17/

# lab 3 db connection
```
docker run -dp 3000:3000 \
  -w /app -v "$(pwd):/app" \
  --network todo-app \
  -e MYSQL_HOST=mysql \
  -e MYSQL_USER=root \
  -e MYSQL_PASSWORD=secret \
  -e MYSQL_DB=todos \
  node:12-alpine \
  sh -c "yarn install && yarn run dev"
 
docker exec -it 54b4d266eef0 mysql -p todos
```
