# cloud-computing-test-vm

eval "$(ssh-agent -s)"

ssh-add labone

docker run -dp 80:3000 getting-started

http://40.81.130.17/
