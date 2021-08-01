# AmzPlayer

AmzPlayer is A Modern Player for Zillions. See http://www.polyomino.com/amzplayer.

Zillions is a player of board games according to rules specified in a ZRF rules file. Mostly games are for two players, human against computer, although single player games (puzzles) are possible too. The Zillions rules file is highly flxeible, convering games from simple tic-tac-toe (or noughts and crosses) through to chess, go and anywhere in between. Games must be of perfect information, so games with hidden cards like poker or bridge are not possible.

Zillions includes a powerful artificial intelligence, which provides a strong opponent across a wide range of games. AmzPlayer provides a modern player that can be published to just about any platform.

# Release

Zillions was released as a Windows program around 20 years ago. This is a re-release of the original Zillions with a modern player built on the Unity platform. It comes with the same standard library of 48 games and many variations.

This is an alpha release, with some changes and limitations. Most recent first.

## Release 3.0-21g30
- fixes a problem with dependencies on .netcore 5.0 and C runtime v142, by including them in the release
- adds move animation and sound (first iteration, needs work).

## Release 3.0-21g12
- there is no move animation or sound (to be done)
- no developer features (authoring mode, etc)
- no support for saved games (to be done)
- no specific support for user-defined games; for now, you can load your own games by editing or replacing the select.zrf file. 
- music files are in OGG format (MIDI not supported)
- sound files are in WAV format, but some sounds will not play because they are in a format that Unity does not accept
- image files are in either BMP or PNG
- Zillons 3.0 introduced some new features to the ZRF format, which may introduce breaking changes (go-moku.zrf fails).

# Licensing

This is free software. You are free to download it, free to use it and free to create games with it, at no charge.
In return, you are expected to provide feedback and report bugs by:
* submitting an issue to https://github.com/david-pfx/AmzPlayer
* email to david@polyomino.com.

# Getting started

- Download and unzip the software. See https://github.com/david-pfx/AmzPlayer/releases. 
- Change directory to Engine and run the AmzEngine.exe. There is a BAT file which does that.
- This should start the player. Enjoy!

# More Detail

This is the original Zillions program heavily modified to run as a server engine, with an all-new Unity player. The original MFC user interface has been removed and replaced by an API and it should play exactly the same as the v3.0 version from which it was derived. The essential features of the user interface have been re-created in Unity, but this has been a complex process, and there will be omissions and differences. This alpha release is intended to identify what still needs to be done. A later release will add core features and platforms.

