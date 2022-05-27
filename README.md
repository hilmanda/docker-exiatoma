<div align="center">

# DOCKER MEMORY-GAME
  
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

# How to Run Container
Clone this repository or download [here](https://github.com/hilmanda/docker-exiatoma/archive/refs/heads/main.zip). 

## Dependencies
Install x server (recommended from VcXsrv) using choco
```
choco install vcxsrv
```

Launch the x server from start menu.

## Execute docker container 
Open the terminal on your PC, then make sure that the current directory is same as directory that you put this repository. To execute the container use command below:
```
docker run --rm -it -e DISPLAY=192.168.1.10:0.0 -v "/d/02-Project/pygame-docker:"/usr/project pygame-docker /bin/bash
```
NOTES!!
You can see that double quote on above, that can be different depend on your directory location.

## Build Docker
Then, you can check first if the repository showed on docker or not by using this command:
```
docker images
```

Next, build the docker file by using command below:
```
docker build -t pygame-docker
```

Finally, the game can be start using container builded using this command:
```
python main.py
```
Alternative command:
```
python3 main.py
python3 -m main.py
```
