# Docker HTK

Docker Image for HTK using a modified source code to fix some building problems.

## Usage

Create a directory structure on your local host machine:

    mkdir -p ASR/MFCCs/train ASR/MFCCs/test \
            ASR/labels/train ASR/labels/test \
            ASR/lists ASR/lib ASR/hmms ASR/results

To get a prompt in the container with your host directory mounted:

    docker run --rm -it -v $(pwd)/ASR:/ASR dgrnwd/htk:latest

