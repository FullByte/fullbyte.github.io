# youtube-dl

Examples using youtube-dl

## Info

|What|Where|
|-|-|
|Official Page||
|Source||
|Download||
|Install|choco install youtube-dl|

## YouTube video download

Download to a specific location in best quality:

```shell
youtube-dl -f 22 -o 'path' '<youtube-link>'
```

Download with details:

```shell
youtube-dl -f 22 --write-description --write-info-json --write-annotations --write-sub --write-thumbnail '<youtube-link>'
```

## Audio only

```shell
youtube-dl -i --extract-audio --audio-format mp3 --audio-quality 0 '<youtube-link>'
```

## YouTube Playlists

Download a playlist:

```shell
youtube-dl -f 22 -i --prefer-ffmpeg --yes-playlist '<playlist-link'
```

Download a playlist with audio only:

```shell
youtube-dl -f 22 --yes-playlist '<playlist-link'
```

## Get Video Source Information

Get Source formats available:

```shell
youtube-dl --list-formats '<youtube-link>'
```