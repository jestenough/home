FROM texlive/texlive:latest

RUN apt-get update && apt-get install -y --no-install-recommends \
    python3 \
    python3-pip \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /app
COPY . /app

ENTRYPOINT ["python3", "compile.py"]
