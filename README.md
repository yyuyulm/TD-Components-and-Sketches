# TD-Components-and-Sketches
## Components & sketches tox

These are some comps for common patterns I created to speed up my work flow, as well as some sketches I made.

### CHOPs.tox
**Compare** 
<br/>
An OP that compare the two inputs, if the second input is not provided then the parameter Cuttoff is used.
<br/><br/>
**Compare_2CH**
<br/>
Similar to Compare, but operates on two channels indivually.
<br/><br/>
**Customs_Fps**
<br/>
An OP that returns the frame count at a custom framerate, used for effects that updates at a different frame rate than main.
<br/><br/>
**Multi_Swtich_Index**
<br/>
An OP that returns the index that wraps around 0-(length-1), increments when a pulse is given to the input. Usually used with any kind of Switch OP.

### TOPs.tox
**Frame_Trail**
<br/>
An OP that composite frame trails with custom number of trailing frames and intervals between them.
<br/><br/>
**Intense_Normal**
<br/>
An OP output an intensified normal output. Use as the sample coord for monochrome noise for a metallic look.
<br/><br/>
**Ramp_From_Texture**
<br/>
Similar to a Ramp Top, but the color ramp is taken from the input. (Constructed with fragmented GLSL pixel shader code are assembled with SwitchDAT and MergeDAT)
<br/><br/>
**UV_Coordinate**
<br/>
Simple GLSL TOP that returns the UV Coordinates.
<br/><br/>
**UV_Lookup**
<br/>
A special case of DisplaceTOP, using the second input.rg as UV to sample the first input.(Better performance than a GLSL implementation)
### Effects.tox
**Film_Defects**
<br/>
Add scratch lines and dust for a filmic look. Can either composite over the input or just use input as resolution source.
<br/><br/>
**Film_Jitter**
<br/>
Glitching effect.
<br/><br/>
**Hand_Drawn_Pencil**
<br/>
A filter that creates a pecil sketch look. Usually, a Edge TOP is used before this.
<br/><br/>
**Ripple**
<br/>
A filter displace the image based on a ripple looking effect.
<br/><br/>
### Sketches.tox
**Edge_Germ**
<br/>
Recursive use of EdgeTOP. Can be used as a backgroud.
<br/><br/>
**Lorenz_Attractor**
<br/>
A simple GPU particle system implemented in GLSL. Keyboard 1 to reset drawing, 2 to reset particle postion, 3 to change camera postion, 4 to reset camera postion, 5 to toggle blur mode.
<br/><br/>
**Recursive_Displacement**
<br/>
Something that resemples a fluid simulation based on SlopeTOP and DisplacementTOP. Warped UV can be used in UV_lookup to warp any image.
<br/><br/>
**Voronoi_Diffusion**
<br/>
Something that resemples a reaction-diffusion simulation based on SlopeTOP and DisplacementTOP. Keyboard 1 to reset simulation, 2 to change noise seed, 3 to swtich between moving noise and static noise (try pressing 3,1,2,2,2....), 4 to turn on camera as input.
<br/>
[See example here](https://youtu.be/8dL384bUOKk&t=1m30s)
<br/><br/>
**Line_Displacement**
<br/>
Inspired by the album cover of Unknown Pleasures by Joy Division. Turn on "Selfie" mode for a astract portrait of yourself (Keyboard 1 to cache snapshots, 2 to save).
<br/><br/>



## Project toe

These are the toe file for my past projects.
<br/><br/>
**Live Music Video**
[Render](https://youtu.be/uZxCMToazwE)
<br/>
[Recording](https://youtu.be/YFhH8oFhrsI)
<br/><br/>
**The Escape**
[Render]()
<br/>
[Recording](https://youtu.be/8dL384bUOKk)
<br/><br/>
