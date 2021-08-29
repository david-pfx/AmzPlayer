# AmzPlayer

AmzPlayer is A Modern Player for Zillions. See http://www.polyomino.com/amzplayer.

Zillions is a player of board games according to rules specified in a ZRF rules file. Mostly games are for two players, human against computer, although single player games (puzzles) are possible too. The Zillions rules file is highly flxeible, convering games from simple tic-tac-toe (or noughts and crosses) through to chess, go and anywhere in between. Games must be of perfect information, so games with hidden cards like poker or bridge are not possible.

Zillions includes a powerful artificial intelligence, which provides a strong opponent across a wide range of games. AmzPlayer provides a modern player that can be published to just about any platform.

# Getting started

- Download and unzip the software. See https://github.com/david-pfx/AmzPlayer/releases. 
- Change directory to Engine and run the AmzEngine.exe. There is a BAT file which does that.
- This should start the player. Enjoy!

# Using the Program

Zillions was released as a Windows program around 20 years ago. 
This is the original Zillions with a modern player built on the Unity platform. 
It comes with the same standard library of 48 games and many variations. 
The Zillions Language Reference should be consulted for any questions about the language and how it works. 
Please be aware that this version was built from a later unreleased version of Zillions 3.0 and there may be slight differences. 

Most features should be self-evident, but please note:
- User games are accessed by clicking on the Polyomino graphic. Edit User.zrf to get access to your games.
- The board can be zoomed in and out using the scroll wheel or Ctrl+plus/minus.
- A move can be made when hovering on a piece by click (if there is only one), by drag and drop to the target position, or by hitting a number key.
- A computer move can be interrupted by Escape or clicking on the board.
- Any game in progress can be saved and restored by clicking a button. Save files are stored in the Saves directory, one per variant.
Please send me the save file if you want to notify a problem.
- Engine DLLs will only be found if they are located in the directory Engine or Engine/Engines (this is a Windows oddity).
- Some problems with sounds have been fixed by substitution. It seems Unity cannot deal with a bit rate of 194 Kbps (default drop and capture).

# Technical Details

This is the original Zillions program heavily modified to run as a server engine, with an all-new Unity player. 
The original MFC user interface has been removed and replaced by an API and it should play exactly the same as the v3.0 version from which it was derived. 
The essential features of the user interface have been re-created in Unity, but this has been a complex process, and there will be omissions and differences. 

# Release

This is an alpha release, with some changes and limitations. 
It is intended to identify what still needs to be done. 
A later release will add core features and platforms.

## Release 3.0-21h30
- adds save, restore, play now
- adds user games
- fix issues with undo/redo, new game
- minor tweaks to scaling and user interface

## Release 3.0-21h13
- fixes scaling of pieces smaller than position
- fixes crash with dummy positions and animations.

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

