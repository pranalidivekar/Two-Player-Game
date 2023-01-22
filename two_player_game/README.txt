# two-player-game
This is an image guessing game between 2 players. The players are supposed to guess the word of the image. For every correct word, a percent of the image will be revealed.
The images are placed on the server. The client requests the server for the image files and they are sent line by line to the client. The game resides and is played on the client. 
The purpose of placing the images on the server was the ease of switching between one/mutiple images. 
The class files used in this program are as follows - 
1. Game.java - the main class that is responsible for switching of players and initiating the game.
2. Player.java - specific to one player 
3. Picture.java the client class that sends the connection request to the server and then reads the image file sent by the server line by line
4. PictureServer.java - server class that receives request for connection from client and sends the requested image file line by line on the connection is made

The execution command is as follows- 
Server command:
java PictureServer -port 80

Client command:
java Game -me sharvai -meWords sharvaiwords.txt -mePicture "prisonmike.txt" -you pranali -youWords pranaliwords.txt -youPicture dwight.txt 80