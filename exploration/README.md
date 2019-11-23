# How to run

1. docker build -t why-fraud-explore .
# 2. docker run -p 8898:8888 -p 9000:9000 -v $(pwd):/app wrangle
2. docker run -p 8898:8888 -v $(pwd):/app wrangle
3. copy/paste the token into browser running on port 8898

# Cleaning up

1. docker rm *VARIOUS IMAGES*
2. docker rmi why-fraud-explore:latest


