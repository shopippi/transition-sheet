## Transiton-sheet

### Transposition is an important concept in music theory. It is used primarily for the following purposes

- Adjustment of vocal range: Transposition helps singers and performers to sing and play in their own vocal range. If a particular song is too high or too low for a singer or instrument, transposition can be used to adjust the range to one that is more comfortable for singing.


- Instrumental Tuning: Some instruments are easier to play in certain keys and more difficult in others. Transposition may be used to adjust the instrument to a key that is easier for the instrumentalist to play.

- Music tonal adjustment: The key of a piece of music can affect the mood and coloring of that piece. For example, playing the same melody in different keys can change the mood of the song. Transpositions can be used to adjust the mood and color of a song.

### Transposition software is a tool that automates these transposition tasks. In general, they offer the following advantages

- Fast and accurate transposition: Instead of manually changing the score, transposition software allows you to transpose a piece of music to another key quickly and accurately.
- Versatility: In addition to transposing a piece of music, transposition software may also include a variety of other features, such as speed changes, voice adjustments, and more.
- Flexibility and convenience: Transposition software allows any key to be selected, allowing performers and singers to play songs in the key that suits them best.

Overall, transposition is an important means of making music more accessible and more comfortable for performers and singers. And transposition software streamlines the process, providing flexibility and convenience.


![image](res.png)

## Developing a Sheet Music Reader
Calvin Gregory, and Calvert Pratt

### I.	Introduction
Applications in the field of Music Optical Character Recognition (OCR), also referred to as Optical Music Recognition, are an application of machine vision which serves to simplify the sight reading learning process and speed up music transcription. The sheet music reader application SheetVision was developed to convert single-tone lines of written music into a computer readable format for audio song playback. It does this through a template image matching algorithm implemented in Python using OpenCV which searches the target image for instances of each music character type such as notes, flats, and sharps. These characters are then identified, sequenced, and exported to a MIDI file for playback. 

### II.	Project Scope
The sheet music reader application was designed to convert images of written sheet music into a computer-readable format. SheetVision takes in an image of written sheet music, classifies all relevant music characters in the image, then generates and exports a MIDI file with all of the classified characters properly sequenced and identified as music notations. The application can handle single tone sequences of notes consisting of whole, half, quarter, and paired eighth (Ti-Ti) notes. It also interprets key signatures (sharp and flat symbols included at the beginning of a line) and rest characters. SheetVision is capable of interpreting most simple to moderate complexity sheet music arrangements written for single-tone instruments such as woodwinds, strings, and vocals. 

### III.	Algorithm
The algorithm used for music character identification uses the following series of steps to categorize each note or symbol in the target image:
 - A.	Image Filtering / Binary Conversion
 - B.	Template Scaling
 - C.	Character Classification
 - D.	Classifier Thresholding
 - E.	Note Identification and Sequencing
 - F.	Export results to MIDI

------------------

#### Libraries sourced from http://www.lfd.uci.edu/~gohlke/pythonlibs/
- (for x64)
  - numpy-1.11.1+mkl-cp35-cp35m-win_amd64.whl
  - matplotlib-1.5.2-cp35-cp35m-win_amd64.whl
  - opencv_python-3.1.0-cp35-cp35m-win_amd64.whl
- (for x86) 
  - numpy-1.11.1+mkl-cp35-cp35m-win32.whl
  - matplotlib-1.5.2-cp35-cp35m-win32.whl
  - opencv_python-3.1.0-cp35-cp35m-win32.whl

Midiutil Python 3 version is included in this repo
