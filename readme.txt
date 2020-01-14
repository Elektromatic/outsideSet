C----------------------------------------------------------------------------
C  			          outsideSet                
C----------------------------------------------------------------------------
C
C  This Pure Data patch creates "generative music" in conjunction with an 
C  electronic synthesizer.
C
C  This patch generates melodies, outside the Mandelbrot set, with random rhythms. 
C  The chaotic values just outside the set are mapped onto a scale to generate
C  musical notes.
C  Please see https://en.wikipedia.org/wiki/Mandelbrot_set for a description of
C  Mandelbrot set.
C  
C  This patch also uses a "quantizer" modeled after Harmonaig Instruo eurorack 
C  module. https://www.modulargrid.net/e/instruo-harmonaig
C  The Instruo module is a chord generating quantizer.
C
C  Please see https://youtu.be/IMkVKST_Wgg for an example of the use of this
C  Pure Data patch.
C
C----------------------------------------------------------------------------
C  Requirements:   Pure Data <https://puredata.info/downloads/pure-data>
C----------------------------------------------------------------------------
C
Usage:  The file outsideSet.pd is the parent patch which contains the 
        rest of the modules.

              Explanation of the primary patches:
midiClockIn:  Generates bangs in sync with an external midi clock 
              from a synthesiser.
quantizer:    This patch models the Instruo by creating four note chords with various
              quality, voicing, and inversions. This patch uses the patches quality, 
              voicing, invert, setctl, and setctl2.
randomRhythm: Creates random rhythms.              

Contributing: Any contributions to this project are welcome.

Acknowledgements: I'd like to thank Acreil for sharing his Pure Data patches.
