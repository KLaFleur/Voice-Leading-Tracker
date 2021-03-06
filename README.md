# Voice-Leading-Tracker

This project is designed to recognize and label internal voice leading lines in melodies. Even though a melody may be played on 1 instrument, one note at a time, it may have multiple discrete voices. This is important because we hear these almost as their own melodies. When there is a skip or jump in the contour of a melody, we seem to wait for when the melody returns to further develop the voice it departed from. 

Here's a possible sample output for the first 2 systems of Bach's Invention #4. When there is a change in voice(as I've defined it) the color changes. The phenomenon where 2 voices are attended to at once is best explained by the second system, where the lower voice(teal) is returned to about once a bar.
![](examples/inv4.png)
## Issues
when 2 internal voices go to the same place, its hard to say which voice takes precedence, or how it would be possible to illustrate that this has occurred.

![](examples/invEx1.png)

When 1 voice (arguably) splits into 2, its hard to show what has happened. It may be best for clarity in this situation to label the note c in bar 9 orange rather than teal.

![](examples/invEx2.png)

## Implementation
This is just a sketch of a project right now, so I'm concerned with 

- Writing or researching a proper definition for when the line departs from a certain voice
  - Ex). If the melody jumps more than a minor 3rd
- Picking the right music notation file type to take as input and manipulate (probably .xml or .sib)
  - .Xml is treated as a generalized notation file, but it may not be able to encode color info
- Possible examples to run through the script.
  - Bach cello suites 
  - Bach inventions (upper melody only)
  - Charlie parker solos