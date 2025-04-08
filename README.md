## Python base image for InfraSonar probes and agents

It is recommended to use a version tag when building probes or agent, so it is clear which version is being used.

Example Dockerfile

```Dockerfile
FROM ghcr.io/infrasonar/python:3.12.9
ADD . /code
WORKDIR /code
RUN pip install --no-cache-dir -r requirements.txt
CMD ["python", "main.py"]
```
