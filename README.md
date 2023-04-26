# Auto-GPT: An Autonomous GPT-4 Experiment (ARM64 Fork)

This is a fork of the original Auto-GPT repository, which showcases the capabilities of the GPT-4 language model. In this fork, we've made some changes and improvements to optimize the project for Apple Silicon and ARM64 platforms.

## Changes in this fork

- Updated Dockerfile for better compatibility with Apple Silicon and ARM64 platforms.
- Optimized some dependencies for better performance on ARM64 platforms.
- Made minor adjustments to the documentation to reflect changes in this fork.

## Setup and Run for Apple Silicon Users

### Prerequisites

1. Install [Docker Desktop for Mac (Apple Silicon)](https://docs.docker.com/desktop/mac/apple-silicon/).

### Building the Docker image

1. Clone this repository to your local machine:

git clone https://github.com/bmills20/Auto-GPT.git
cd Auto-GPT

2. Build the Docker image for the Apple Silicon platform:
docker build --platform linux/arm64 -t arm64-autogpt --build-arg BUILD_TYPE=dev .

### Running the Docker container

1. Run the Docker container with the following command:

docker run -it --rm -v "$(pwd)/data:/app/data" --name autogpt-instance arm64-autogpt


This command will create a Docker container named `autogpt-instance` and mount the local `data` folder inside the container's `/app/data` folder.

## Features, Requirements, and Quickstart

Please refer to the [original README](https://github.com/Significant-Gravitas/Auto-GPT/blob/master/README.md) for information on the features, requirements, and quickstart guide for Auto-GPT.

## Contributing

If you'd like to contribute to this fork, feel free to open a pull request or raise an issue with your suggestions or improvements.

## Acknowledgements

We'd like to thank the original developers and contributors of Auto-GPT for their hard work in creating this experimental application. This fork aims to build on their work and make it more accessible to a wider range of platforms.
