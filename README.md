# k8s-hw2

## before you start:

create `.env` file inside of the kubernetes folder and set appropriate environment variables. Afterwards, inside of the kubernetes folder run the following command:

```
    kubectl create secret generic mern-secret --from-env-file=./.env   
```
then

```
    kubectl apply -f . 
```

## credits

For educational purposes I have used a @bjnandi project.
Thanks [@bjnandi](https://github.com/bjnandi) for the [solution](https://github.com/bjnandi/containerize-full-stack-app-MERN-with-docker-compose) implemented with the MERN stack
