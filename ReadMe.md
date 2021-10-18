# AmzPlayer

AmzPlayer is A Modern Player for Zillions of Games. See http://www.polyomino.com/amzplayer.

Mostly the games it can play are for two players, human against computer, with everything out in the open (no hidden cards). 
That includes a wide variety of games from simple tic-tac-toe (or noughts and crosses) through to Chess, Go and anywhere in between. 
It includes many games of historical interest, and games not widely known that are still very playable.
Single player games (puzzles) are possible too.

The software includes a powerful artificial intelligence in the form of a computer opponent that can be a real challenge to beat.

# Getting Started

- Download and unzip the software. See https://github.com/david-pfx/AmzPlayer/releases. 
- Change directory to Engine and run the AmzEngine.exe. There is a BAT file which does that.
- This should start the player. Enjoy!

# Using the Program

Select a game from the select screen by clicking on a tile image.
Additional games are found by choosing a different select variant.
A small selection of user games can be accessed by clicking on the Polyomino graphic. 

Moves can be made in several different ways.
- Click on an empty space to drop a piece there. 
A preview of the piece to be dropped will appear flashing.
- Drag a piece to move it to a space indicated by a flashing circle.
- Click on a square a piece can move to.
The piece to be moved and a flashing circle will preview the move.

In each case, if there is more than one possibility, move the mouse cursor until the move you want appears in the window before clicking.
Alternatively hit a number key to pick that move.

Most other features should be self-evident, but please note:
- A right click will provide additional information about available variants, rules for a game or piece.
- The board can be zoomed in and out using the scroll wheel or Ctrl+plus/minus.
- A computer move can be interrupted by Escape or clicking on the board.
- Flipping the board leaves you in control of all players.
Play your move and then hit the computer play button to continue.
- Any game in progress can be saved and restored by clicking a button. 
Save files are stored in the Saves directory, one per variant.
Please supply the save file if you want to notify a problem.
- User games are accessed by clicking on the Polyomino graphic. 
- Edit SelectUser.zrf to get access to your own games or those you download.
- Engine DLLs will only be found if they are located in the directory Engine or Engine/Engines (this is a Windows oddity).

# Known problems

The following are known problems which may be corrected in a later release.
- The engine used for Reversi may not terminate until you tell it to 'play now'.
- Some problems with sounds have been fixed by substitution. 
It seems Unity cannot handle MIDI files or WAV files with a bit rate of 194 Kbps (default drop and capture).
- The supplied version of one game (Go Moku) did  not compile.
It was a new 3.0 version, and has now been replaced by the original 2.0 version.
- Games that offer a very large number of move choices may not be playable with the current move selection mechanism.
Please supply an example if you have one.
- Games with a very large board may not be playable, because the board can be zoomed but not scrolled.
Please supply an example if you have one.
- Some Zillions features including hints, printing, author mode and some display details have not been implemented (yet).

# Technical Details

Zillions was released as a Windows program more than 20 years ago, and abandoned by about 2005. 
This is the original Zillions code base heavily modified to run as a server engine, with an all-new Unity player. 
This version was built from a later unreleased version of Zillions 3.0, so there may be slight differences in behaviour. 

The Zillions Rules File is a programming language for specifying board games. 
While it can handle many games of chance, they must be games of perfect information, so games with hidden cards like poker or bridge are not possible.
The Zillions Language Reference should be consulted for any questions about the language and how it works. 

# Release

This is an alpha release, with some changes and limitations. 
It is intended to flush out bugs and identify what still remains to be done. 

## Release 3.0-21j18
- new look with larger board
- new select games structure
- improvements to preview and move selection
- right click information

## Release 3.0-21i17
- piece sets, flip board, player selection
- face and search results
- saved preferences
- better animations and move selection
- solutions and progressive variants

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

