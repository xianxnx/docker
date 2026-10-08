FROM debian
RUN apt-get update && apt-get install -y stress && rm -rf /var/lib/apt/lists/*
CMD ["bash", "-c", "stress -c 2"]
