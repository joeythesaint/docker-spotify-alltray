# Dockerized Spotify

Run Spotify inside an isolated [Docker](http://www.docker.io) container. This is achieved by sharing a socket for X11 and PulseAudio.

## Instructions

1. Clone this repository and change to the directory:

  ```sh
  git clone https://github.com/terlar/docker-spotify-pulseaudio.git && cd docker-spotify-pulseaudio
  ```

2. Build the container:

  ```sh
  sudo docker build -t spotify .
  ```

3. Run the container with the appropriate volume mappings:

  ```sh
  docker run --rm --name spotify \
		-v /tmp/.X11-unix:/tmp/.X11-unix:ro \
		-v /run/user/$(id -u)/pulse:/run/pulse:ro \
		-v ${HOME}/.spotify/config:/data/config \
		-v ${HOME}/.spotify/cache:/data/cache \
		--device /dev/dri spotify
  ```

4. Use Spotify.
