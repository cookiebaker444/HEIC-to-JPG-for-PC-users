Make sure install python first on your device:
https://www.python.org/

Recommended IDE to run this python code:
Visual Studio Code
https://code.visualstudio.com/

Install Docker for Windows from here:
https://docs.docker.com/desktop/setup/install/windows-install/

Install Docker on Mac:
1. Make sure Homebrew is installed
2. Run the following command in terminal: ```brew cask install docker```

After Docker is installed locally, make sure Docker is running, and run these command to make sure the image is built and then the container is started:

1. ```docker build -t heic_converter .```
2. ```docker run --rm -v $(pwd):/app heic_converter``` (If running on MAC)
3. ```docker run --rm -v %cd%:/app heic_converter``` (If running on Windows PC)

HEIC photos should be stored in the same folder as the python code and the Dockerfile.

When test running the code, the heic file included in the folder should be converted to jpg file in the same folder.
