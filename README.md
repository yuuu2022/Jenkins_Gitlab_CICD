# Jenkins_Gitlab_CICD
try to complete a task with CICD .
- complete a development and test with CICD as below steps
  1. develop springboot project
  2. commit to gitlab
  3. jenkin pull the source
  4. jenkin set task to run the maven script to build the jar
  5. pass the jar to docker 
  6. write dockerfile to run the jar in docker
  7. write docker compose to run the jar
  8. test the jar in docker container
  9. run the jar to production env after the test
      
installation of gitlab:

1. docker pull gitlab/gitlab-ce
2. sudo docker run --d \
  --hostname gitlab.example.com \
  --p 8443:443 --p 8980:80 --p 8922:22 \
  --name gitlab \
  --restart always \
  --volume $GITLAB_HOME/config:/etc/gitlab \
  --volume $GITLAB_HOME/logs:/var/log/gitlab \
  --volume $GITLAB_HOME/data:/var/opt/gitlab \
  --shm-size 256m \
  gitlab/gitlab-ce:latest


