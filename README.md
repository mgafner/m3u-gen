# m3u-gen
Bash script for creating m3u-playlist files

## About m3u-gen
i am using the identifier "tag" as same as "playlist"
my playlists are generated out of "tags" which i am writing in the 
comment-field of mp3-files. For example:
comment: Rock; Pop; Schlager; 

for each playlist btw comment-field we can declare a [section]
each section may have optional settings:
exclude_tags
exclude_ratings
exclude_artists
include_tags
include_ratings
include_artists

m3u-gen works recursive on every file in a given directory
the working order of given settings is as seen in the settings list above.
first we can exclude songs, then we can include some again

Beware: It works on mp3 files and writes mp3-tags! Check the code before using it!

## Installation
#### Prerequisites
   * eyeD3 grep sed awk

#### Debian / Ubuntu
```
sudo apt-get install eyeD3 grep sed awk
```

## Usage
```
usage:
copy rules.example to rules
edit rules for your needs
edit m3u-gen and change the path for mp3-directory and playlists
start m3u-gen

```

## License
m3u-gen is free software, available under the [GNU General Public License, Version 3](http://www.gnu.org/licenses/gpl.html).

