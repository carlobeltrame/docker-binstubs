# Ruby and rake in a Docker container

Usage:
```bash
docker run -it --rm -v $(pwd):/app carlobeltrame/ruby ruby <something>
docker run -it --rm -v $(pwd):/app carlobeltrame/ruby rake <something>
```

How to push (note to self):
```bash:
docker build -t carlobeltrame/ruby:latest .
docker run carlobeltrame/ruby:latest ruby --version
docker build -t carlobeltrame/ruby:<version of vue cli> .
docker push carlobeltrame/ruby:<version of vue cli>
docker push carlobeltrame/ruby:latest
```