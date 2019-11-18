# DJTS-Saves
Save data analysis for the THQ DS game Drake &amp; Josh: Talent Showdown, viewable [here](https://eiim.github.io/DJTS-Saves/).
## What is this?
This tool analyzes raw .SAV or .dsv save files for Drake &amp; Josh: Talent Showdown.
It analyzes every byte or group of bytes known to be set in regular gameplay, giving human-readable results. The info provided includes checksums, Joshakazam details, settings, guitar level high scores, save dates, save progress, etc.
There is little practical use for this tool, I simply made it to analyze saves for interesting info more rapidly.
## How can I use it?
Really? You want to use this? Well, I suppose...
You'll need to get a raw save file. In most emulators, this is stored in the "Battery" folder, titled with the name of the game. Note that some emuators, such as no$gba, will automatically compress save files. You'll have to turn this off for them to be legible here.
Then, simply select the file with the "Choose file" button. It doesn't upload it to any servers or anything, it's all client-side because you're only parsing like 200 bytes.
## How can I help?
If you come across an issue, open an issue or pull request.
If you want to help with save data analysis, here's a few open questions:
* Bytes 0x58/0x88/0xB8 (which have something to do with the first two digits of the year) aren't totally understood yet.
* The 5-byte header is always constant, but we have no idea what it means
* Most importantly, there's 5 checksums which we can't figure out. They don't seem to be CRC-32 or anything nice and simple like that. If you know how to reverse checksums, let me know and I'll send you example data.