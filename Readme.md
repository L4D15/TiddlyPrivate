# Private Tiddlywiki Template

This is a regular Tiddlywiki installation with added functionality to export two different types of outputs:

* Private: Contains all tiddlers.
* Public: Contains all tiddlers except those with the `Private` tag.

This in situations where you want to publish the content of the Tiddlywiki but conceil some of the information. I use it in my role-playing game sessions, so I can build the world and reveal details about it to my players publishing an online --censored-- version to maintain the intrigue.

## Requirements

Requires [Node.js](https://nodejs.org/en/) the [TiddlyWiki](https://github.com/Jermolene/TiddlyWiki5) server installed in the system.

## Usage

1. Clone this repository.
2. Navigate to the root directory and start the Tiddlywiki server with `tiddlywiki . --server`.
3. Navigate to http://127.0.0.1:8080/ in your browser and use Tiddlywiki as usual.
4. Run `tiddlywiki . --build private` to create a full local private version with all tiddlers at `./private`.
5. Run `tiddlywiki . --build public` to create a public version without the private tiddlers at `./public`.
6. Publish your public Tiddlywiki to [Tiddlyspot](http://tiddlyspot.com/) or your favourite hosting service.
7. Profit.

Thanks to [Sukima](https://github.com/sukima) for the script to filter the tiddlers and [Jermolene](https://github.com/Jermolene) for such an awesome tool as [TiddlyWiki](https://github.com/Jermolene/TiddlyWiki5).
