#### Technology Tools Stack

```
1. Java-17
2. Maven
3. Docker
4. Docker-compose
5. Postman
6. PostgreSQL
7. Redis
8. k8s 
9. kubectl
```

#### Building and Running Application with Docker

```
mvn clean package -DskipTests
```

```
docker compose up -d java_db
```

```
docker compose up -d java_app
```

#### Running application with kubernetes or cloud

```
1. Update the value for `configMap` and `secret` according to your environment in `k8s_deployment.yaml' file.

2. Apply or create the deployment by `k8s_deployment.yaml` file with below command with kubectl cli.

3. Kubectl apply -f k8s_deployment.yaml
```

#### Testing the application

1. GET request
   
   ```
   http://localhost:8081/api/users
   ```

2. POST request
   
   ```
   http://localhost:8081/api/users
   {
       "name" : "Sawan"
       "email": "devOps@gamil.com"
   }
   ```

3. DELETE request
   
   ```
   http://localhost:8081/api/users/{user_id}
   http://localhost:8081/api/users/1
   ```
