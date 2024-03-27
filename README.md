# SepctroMania: An All-In-One Audio Management & Analysis Software

## What is it?
SpectroMania will be a FLOSS audio management program that allows the user to work with audio files within a simple command-line (with future GUI planned) interface. The purpose behind this software is to facilitate common audio management tasks into a single, streamlined solution that includes most frequently used tasks and features into a common workflow.

The features I have planned for this application include:
- Transcode audio files through multiple formats (mp3, flac, aac, etc).
- Append missing id3v2 metadata to selected audio files (with batched files support planned) either through an online database and API requests, or by having the user manually enter information themselves. The software will also allow for album artwork support.
- Check audio file quality integrity (more information covered below).

## My plans:
The first step is learn more about the libraries needed for the software to function. This includes ffmpeg for transcoding audio files, and libtag or libid3tag for appending metadata to audio files. The second step will be used for enhancing the second feature by doing some research on globally avaialbale databases that contain information on every track recorded and has an API that allows for data retreival based on the name of a track, so that users can import any track through the software, and have a query with the name of the track be sent with returning results on potential matches, so that the user may choose which track is the right one and have the software tag their track accordingly.

After developing the software, a Qt-based graphical user interface will be planned to allow for an enhanced user experience for those who are not versed into the command line and would prefer using a standard window to interact with the software.

## Why?
Throughout the years I have been collecting scores and recording sessions from some of my favourite movies, and I noticed that some of the tracks do not sound as well as they could. The audio was either lacking base, in an undesired format, or would be encoded in a lossless format that would not equate to the original quality of the track. Both lossless and lossy formats only allow up to a certain frequency range for sound data, and lossy formats tend to cut off at mid frequencies (16-18 hertz), whereas lossless formats go up to 20-22 hertz. It is possible to determine the true quality of the track by first converting the supposedly original file to a lossy format, then evaluate what is the highest frequency it can reach, and if it equals that of the original file, then it would be safe to assume that the original file was transcoded to a lossless format to appear as high quality, when in reality, some of the data from the original recording is not preserved. This feature is what I call file quality integrity.

I have been editing audio and learning about varius terminologies for a couple of years now, with some of my work visible on YouTube, and my experience has led me to think about clever ideas that could simplify my workflow and also be an accessible tool to others who intend to do similar things as me. Obviously, the scope of the tool is limited, and not many features are planned. This tool will also serve as an opportunity to refine my coding skills and gain some valuable insights along the way. More features will be considered based on a variety of factors including spare time, motivation, and public demand.
