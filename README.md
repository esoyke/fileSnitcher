# FileSnitcher

A file-monitoring app built on mbabauer's pub/sub <a href="https://github.com/mbabauer/meteor_publicationsDemo">demo</a> leveraging <a href="https://github.com/paulmillr/chokidar">chokidar's</a> file wrapper.

File Snitcher records when files are added, changed, or removed, as well as the users logged into the system at the time (*nix/OSX supported).

## Usage
Clone repo, set desired watch directory in getFolder() method in server/publish/files.js, fire up meteor and browse to localhost:3000. Changed files display as yellow, deleted as red.

## TODO:
* Make watch directory configurable from client
* Allow specification of excluded sub-directories
* Switch user listing to tooltips

## Issues:
* May not display multiple users correctly (still need to test this condition)