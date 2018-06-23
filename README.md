# CSIRO_auralisation
Some sounds generated during my internship at CSIRO. These are from elderly's activity values of Smarthome.  
The sounds can be generated automaitcally from codes (Python & midiutil etc.).  

## generation
Sounds from raw values and new generated sounds are uploaded.
Even though, activity pattern cannot be inferred from the sounds at this stage (which would make it truly useful), it sounds pretty good!?
This is achieved mostly by  
 
    1. categorising the raw value sounds  
    2. extract their "contour" information, and do some manipulation  
    3. apply tonality and some additional rules to the manipulated contours  
    4. these contours are converted to notes  
        - notes converted to midi files with Python's midiutil library  
        - midi files converted to mp3 with FluidSynth on Ubuntu (with FluidR3_GM soundfont)  

"Contours" is pretty much [current note value]-[previous note value] of raw notes values.   
I think it's actually called something else in music theory, but I forgot what it is.   

I'm not uploading the code since I signed an agreement. May be I will after a few years, if I had to.  
Right now, this repo could serve as a showroom.  

## some ideas
Currently, we only use major tonality (C or otherwise). Using other tonality like minor etc. will give a different feelings to the sounds.
This can be used appropriately if we can extract activity information from raw values.
#### note 1
If I write detailed explanation, it will probably be convoluted since I have to keep finding new words to describe some abstract features,
which doesn't have an analogue to what most people know (?).
#### note 2
If you are reading this, thanks Son and Qing for opportunities. I hope I at least gave you guys some ideas.