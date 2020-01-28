# Running Gogs Git Repo With Docker Compose

This uses docker volumes for persistent storage for both mysql and gogs.

We're using docker-compose to bring up the entire stack which simplified networking.

Get it up and running using the following (note be in this directory when you run this command)

  #Set the mysql root password in the environment
  $export MYSQL_ROOT_PASSWORD=supersecrepassword

  #Bring up the containers.
  $docker-compose up 

This will build all the containers, create volumnes, create the network and bring up the app


After the first time, you can simply run to bring the stack up

  $docker up

To stop it you can simply run the following to bring it down

  $docker stop


Add additional configuration steps
  - [ ] Gogs username: dsoadmin
  - [ ] Gogs Password: password
