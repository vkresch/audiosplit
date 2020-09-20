# AudioSplit

AudioSplit is a C++ program which enables users to split a huge mp3 file into small mp3 files.

## Usage
Download a mp3 file from youtube:

```bash
$ youtube-dl --extract-audio --verbose --audio-format mp3 "https://www.youtube.com/watch?v=2Q6vj1EKUBE"
```
`playList.plyl`:
```
00:00 - Listen To Eurobeat - (Tokyo Future)
05:19 - Never Gonna Give You Up - (Rick Astley) - (Akyra Mix)
10:15 - Blood On Fire - (GO 2 / Christine)
14:35 - Hero Samurai - (Alphatown 2000)
19:09 - Take Me - (Ken Blast)
22:09 - Butterfly - (Hyper K Remix)
25:07 - Invisible Touch - (Fastway)
28:23 - Love Countdown - (Fastway)
32:05 - New Horizon - (Ken Blast)
35:38 - Tekno Samurai - (Mark Foster)
40:03 - Hai Hai Hai - (Marko Polo)
44:27 - Deceptive - (Odyssey)
47:56 - Dont Stop The Music 2019 - (Dave Rodgers)
51:52 - Eye To Eye - (Odyssey)
55:46 - The Element Of Fire - (Fastway)
59:08 - Go Racin Go - (Fastway)
01:02:20 - Make Or Brake - (Fastway)
```

```bash
$ ./audiosplit --file super_eurobeat_vol8.mp3 --playlist playList.plyl --type mp3
```

Result:
```bash
$ ls

Listen To Eurobeat - (Tokyo Future).mp3
Never Gonna Give You Up - (Rick Astley) - (Akyra Mix).mp3
Blood On Fire - (GO 2 / Christine).mp3
Hero Samurai - (Alphatown 2000).mp3
Take Me - (Ken Blast).mp3
Butterfly - (Hyper K Remix).mp3
Invisible Touch - (Fastway).mp3
Love Countdown - (Fastway).mp3
New Horizon - (Ken Blast).mp3
Tekno Samurai - (Mark Foster).mp3
Hai Hai Hai - (Marko Polo).mp3
Deceptive - (Odyssey).mp3
Dont Stop The Music 2019 - (Dave Rodgers).mp3
Eye To Eye - (Odyssey).mp3
The Element Of Fire - (Fastway).mp3
Go Racin Go - (Fastway).mp3
Make Or Brake - (Fastway).mp3
```

## Changelog

0.0.1 First working prototype
