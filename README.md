# fmedia-Audio-Codec-Comparison-Database
This database was created for Evaluation of Audio Compression Codecs.

This dataset contains benchmarks of various audio codecs (FLAC, MP3, AAC, etc.) across different songs, including bitrate, compression ratio, encode/decode time, and speed.

|METADATA|
|---------|
|Track name|
|Artist|
|Genre|
|Uncompressed file size (bytes)|
|Samples no.|
|No. of Bit per channel / sampling rate|
|Bitrate (kbps)|

Table belows shows the audio codecs and settings that was used

| Codec  | Settings |
| ------------- | ------------- |
| FLAC  | VBR level 6  |
| MP3  | CBR 320kbps |
| MP3  | CBR 128kbps  |
| AAC  | CBR 256kbps  |
| AAC  | VBR level 5  |
| Vorbis  | VBR level 7  |

After encoded and decoded each track, bitrate (kbps) (for codecs that use varible bit rate), compressed file size (bytes), and encode/decode time (seconds) were recorded. The compression ratio (%), encoding and decoding speed (samples/μs) were calculated with the formulas below and documented in this database.

Compression ratio (%) = ((Uncompressed file size) / (Compressd file size)) * 100

Speed (samples/μs) = (2*Sample size)/(Recorded time * 1000000)

# How to Contribute
1. Fork this repository
2. Add your song entry to the CSV file
3. Submit a pull request (PR) with your changes
