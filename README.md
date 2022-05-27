<div align="center">

# MEMORY-GAME
> Containerize PyGame with Docker.
  
  <a href="https://www.pygame.org/"><img alt="PyGame" src ="https://camo.githubusercontent.com/1971c0a4f776fb5351c765c37e59630c83cabd52/68747470733a2f2f7777772e707967616d652e6f72672f696d616765732f6c6f676f2e706e67" width = 180 height = 100></a>
</div>

## Nama dan NIM Anggota Kelompok
| Nama | NIM |
| :---: | :---: |
| Jesika Putri               | 120140050 |
| Hilmanda Panji Orienski    | 120140130 |
| Bilhaq Avi Dewantara       | 120140141 |
| Gery Melia Suwanda         | 120140147 |
| Fadhilah Fauza Hamda       | 120140153 |
| Chaterine Sidabutar        | 120140199 |

# Description
This is an food-base memory tile game. The objective of this game is aims to hone one's memory by giving a game in the form of cards that are matched with pictures. The user must find a card with the same food picture and then click simultaneously so that the card is paired. The higher the level, the faster the time, so the user must play and analyze which images are the same. 
Are you ready for this game? Let's complete the level and prove your skills!

# How to Run From Docker (WINDOWS)
Clone this repository or download [here](https://github.com/hilmanda/docker-exiatoma/archive/refs/heads/main.zip). 

## Dependencies
1. Download and Install x server (recommended VcXsrv) from [here](https://sourceforge.net/projects/vcxsrv/files/latest/download).

2. Launch the X Server from start menu.
<div align="center">
  <img src="https://user-images.githubusercontent.com/90018036/170707241-cb5753d5-302f-4c7e-be0b-fb24658d5bd5.png">
</div>
3. Go with all the default settings, however don't forget to check “Disable access control”.
<div align="center">
  <img src="https://miro.medium.com/max/1400/1*ihco-ShEHQtbwHBGmtIOZg.png">
</div>

## Build Docker

1. Make sure your Docker is Running
2. Build the docker file by using command below:
```
docker build -t pygame-docker .
```

3. Then, you can check if the repository showed on docker or not by using this command:
```
docker images
```

## Execute docker container 
Open the terminal on your PC, then make sure that the current directory is same as directory that you put this repository. To execute the container use command below:

```
docker run --rm -it -e DISPLAY=192.168.1.10:0.0 -v "/d/02-Project/pygame-docker":/usr/project pygame-docker /bin/bash
```

NOTES!!
1. You can see that double quote on above, that can be different depend on your directory location.
2. You has to change the DISPLAY IP Address to your own IP


## Run the Game
Finally, the game can be start using container builded using this command:
```
python main.py
```
Alternative command:
```
python3 main.py
python3 -m main.py
```

# DEMO CONTAINER VIDEO
[![HERE THE TUTORIAL](http://i3.ytimg.com/vi/38uOm7qAVD8/hqdefault.jpg)](https://youtu.be/38uOm7qAVD8)
