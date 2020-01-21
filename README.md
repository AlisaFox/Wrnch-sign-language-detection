# Sign Language Translator
Our project uses Wrnch hand-joint detection to identify letters of American Sign Language. It performs its functions by taking an image of a right-handed signer and runs it in word.py.
The image that is being processed will look like the following diagram after it is analyzed using the WrnchAI program:

![sign language a](annotated_media-a[1].png)

Then, the corresponding letter in the English Alphabet will be printed on the console.

We used [wrnchAI](https://devportal.wrnch.ai/wrnchcloud) to get the annotated media and json file.  

#### Methodology

We used the relative distances between hand joints to identify possible translations to the English Alphabet. 
For example:
  - if the index and middle fingers are crossed, we have r
  - if all the fingers other than the thumb are straight and pointed up, we have b
  - and so on (w/ three fingers, different 'levels', etc)

#### Order of elimination:
r, o,

b,

f, w, k

u, v, 

l, d , z, y, i , j

h, p, g, q

t, c, x, n, m, a, e, s

#### Future Plans for Improvements
- implement a front-end version such as a GUI interface
- utilize live video for the annotated media work-type
- apply the program to both right-handed signers and left-handed signers
- implement the program in 3d coordinates to accommodate for slight changes in positioning
