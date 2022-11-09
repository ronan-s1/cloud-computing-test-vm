# cloud-computing-test-vm

ssh -i lab1 ronan-s@40.81.130.17

eval "$(ssh-agent -s)"

ssh-add labone

docker run -dp 80:3000 getting-started

http://40.81.130.17/

# lab 3 db connection
```
docker run -d \
     --network todo-app --network-alias mysql \
     -v todo-mysql-data:/var/lib/mysql \
     -e MYSQL_ROOT_PASSWORD=secret \
     -e MYSQL_DATABASE=todos \
     mysql:5.7
 
docker exec -it 54b4d266eef0 mysql -p todos

docker run -dp 80:3000 `
  -w /app -v "$(pwd):/app" `
  --network todo-app `
  -e MYSQL_HOST=mysql `
  -e MYSQL_USER=root `
  -e MYSQL_PASSWORD=secret `
  -e MYSQL_DB=todos `
  node:12-alpine `
  sh -c "yarn install && yarn run dev"
```
