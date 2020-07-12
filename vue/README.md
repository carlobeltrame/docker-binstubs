# Vue CLI in a Docker container

Usage:
```bash
docker run -it --rm -v $(pwd):/app carlobeltrame/vue-cli vue create
```

How to push (note to self):
```bash:
docker build -t carlobeltrame/vue-cli:latest .
docker run carlobeltrame/vue-cli:latest vue --version
docker build -t carlobeltrame/vue-cli:<version of vue cli> .
docker push carlobeltrame/vue-cli:<version of vue cli>
docker push carlobeltrame/vue-cli:latest
```