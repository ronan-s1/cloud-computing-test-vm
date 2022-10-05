# cloud-computing-test-vm

eval "$(ssh-agent -s)"
ssh-add labone
docker run -dp 3000:3000 getting-started
