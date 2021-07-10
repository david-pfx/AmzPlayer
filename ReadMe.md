# AmzPlayer

AmzPlayer is A Modern Player for Zillions. See http://www.polyomino.com/amzplayer.

Zillions is a player of board games according to rules specified in a ZRF rules file. Mostly games are for two players, human against computer, although single player games (puzzles) are possible too. The Zillions rules file is highly flxeible, convering games from simple tic-tac-toe (or noughts and crosses) through to chess, go and anywhere in between. Games must be of perfect information, so games with hidden cards like poker or bridge are not possible.

Zillions includes a powerful artificial intelligence, which provides a strong opponent across a wide range of games. AmzPlayer provides a modern player that can be published to just about any platform.

# Release

Zillions was released as a Windows program around 20 years ago. This is a re-release of the original Zillions with a modern player built on the Unity platform. It comes with the same standard library of 48 games and many variations.

This is an alpha release, with some changes and limitations.

- there is no move animation or sound (to be done)
- no developer features (authoring mode, etc)
- music files are in OGG format (MIDI not supported)
- image files are in either BMP or PNG
- some upgrades to the ZRF format, which may introduce breaking changes (go-moku.zrf fails)
- support for user-defined games and saved games is not yet implemented. 

# Licensing

This is free software. You are free to download it, free to use it and free to create games with it, at no charge.
In return, you are expected to provide feedback and report bugs to david@polyomino.com.

# Getting started

- Download and unzip the software. 
- Run the AmzEngine.exe. It will start the player.

Enjoy!

# User created games

For now, you can load your own games by editing or replacing the select.zrf file. 

# More Detail

This is the original Zillions program heavily modified to run as a server engine, with an all-new Unity player. The original MFC user interface has been removed and replaced by an API and it should play exactly the same as the v3.0 version from which it was derived. The essential features of the user interface have been re-created in Unity, but this has been a complex process, and there will be omissions and differences. This alpha release is intended to identify what still needs to be done. A later release will add core features and platforms.

