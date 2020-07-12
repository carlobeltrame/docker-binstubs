# char-rnn in a Docker container

Usage:
```bash
docker run -it --rm -v $(pwd):/root/torch-rnn/data carlobeltrame/char-rnn
```

How to push (note to self):
```bash:
docker build -t carlobeltrame/char-rnn:latest .
docker push carlobeltrame/char-rnn:latest
```