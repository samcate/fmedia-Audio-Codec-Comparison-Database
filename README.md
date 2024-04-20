# fmedia-Audio-Codec-Comparison-Database
This database was created for Evaluating Audio-Compression Techniques, and reference to Simon Zolin's work https://stsaz.github.io/fmedia/audio-formats/

More than 50 music tracks from a wide variety of genres were encoded by multiple audio codecs. All tracks include:

|METADATA|
|---------|
|Track name|
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

NOTE: 

-The .xlsx file uploaded is only temporary. A JSON query of the file will be implemented in the future

-AAC cannot encode tracks that has a sampling rate above 96kHz. So all tracks that have higher sampling rate than 96kHz was down-sampled
