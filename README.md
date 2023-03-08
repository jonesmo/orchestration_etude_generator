# Etude Generator for Orchestration Students

#### Video Demo:

#### Aspirational Description:

I'm a composer in my free time. From 2021 to 2022, I took orchestration lessons, during which my teacher
had me write short etudes to study the sounds of different instruments. Together, we hatched the idea of a simple
piece of software that would suggest etudes for orchestration students (eg, write a five-measure chorale for just high-register bassoon,
clarinet, and viola; or, write an angular rhythmic passage for two pitched percussion instruments). This tool could be customized
for composition students working on different goals. For example, you could limit the suggested instruments to only
a certain group or family (strings, percussion) or require all the etudes generated
to include, for example, an oboe. You could even have custom lists of instruments provided by the user.
You could also have it suggest affects or textures ("choppy," "driving," "sparse") in the form of adjectives.
Optional features could include suggestions of keys, alternative tuning systems, tempos, and time signatures.

Another optional feature is a random audio file picker; this tool would access the user's local file system
and select a random .wav file from the specified folder. This can be useful for composition exercises with electronics
and to select random clips of sounds to emulate with acoustic instruments.

The vision for this software is to test it well enough and make a friendly enough interface for it
that I could pass this tool off to my former teacher, who is not a programmer, or any other composer,
and they could use it to generate exercises for themselves or their students. It's sort of like fortune
cookies or Tarot cards to spark ideas for etudes.

#### Features (not all may get done):

- inputs

* takes in a fixed number of instruments for the etude
* takes in a numeric range of instruments, too, and randomly selects an ensemble size
* takes in an instrument family or ensemble
* takes in a list of required instruments that must be part of every etude (error if this is smaller than the ensemble size)
* takes in a custom list of instruments not pre-defined

- pre-defined data

* instrument families and common instruments for each family
* common instruments for common ensembles (string quartet, Pierrot ensemble, piano quintet, etc.)
* list of adjectives: sparseness/denseness, affect, textural, common Italian descriptors
* list of possible keys
* list of possible alternative tuning systems
* list of possible general tempos (adagio, lento, allegro, etc.)

- generators

* tempo
* time signature

- random audio file picker

* access a folder on local file system and all .wav files (only) in that folder (max length, probably 30 or 60 seconds?)
* return some kind of audio player with that file open

#### Steps:

1. Make a database for all the pre-defined data
2. Decide on an interface for all the inputs
3. Create tempo and time signature generators (should be easy and fun?)
4. In consultation with teacher, put all pre-defined data into the database
5. Make interface
6. Connect interface to database (could be hard and not-fun?)
7. Validate user input
8. If time left, start on random audio file picker
9. Decide how to package this thing up for distribution
