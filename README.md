# CS3700 Project 2: Sample FTP Client
David Malone

## High-Level Approach
I ended up following the checklist at the bottom of the assignment page to a tee: I began by writing code to parse the commandline arguments, and then progressed to connecting to the FTP server. Then I moved onto the ```mkdir``` and ```rmdir``` commands since they didn't need a data channel, followed by the ones that did. I finished with testing.

## Challenges Faced
I had a hard time differentiating receiving information from the data channel and the control channel, but looking through Piazza posts to see how each terminated. In addition, I had a particular issue downloading from the server: I kept trying to look for libraries/functions in any package I could think of to create binary files, and each solution just kept returning a "No such file or directory error." I ended up manually creating a file via an external system call, and then opening and writing to it using the ```open``` and ```write``` commands.
