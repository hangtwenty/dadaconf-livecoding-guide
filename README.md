<h3 align="center">
 👁 https://github.com/terkelg/awesome-creative-coding 👁 
</h3>
 
<h4 align="center">
 👁 https://github.com/lvm/awesome-livecoding 👁 
</h4>

----

[github topic: creative-coding](https://github.com/topics/creative-coding)

----

# Dadaconf, meet live-coding

This doc is for [a workshop at Dadaconf 0.1](http://dadaconf.com/workshops.html). Two topics:

1. Livecoding to produce sound — by [hangtwenty](https://github.com/hangtwenty). Sonic Pi and such.
2. [Livecoding to produce visuals](#livecoding-to-produce-visuals) — by [kevincairo](https://github.com/kevincairo). Shaders and such, including a editor+visualizer that runs in your browser and lets you code visuals that respond to sound/music

# [Livecoding](https://en.wikipedia.org/wiki/Live_coding) to produce **sound**

I was introduced to "programming to produce sound" by learning some [Max](https://en.wikipedia.org/wiki/Max_(software)) (as in "Max/MSP" and ["Max4Live"](https://www.ableton.com/en/live/max-for-live/)). (Related: [Pure Data aka Pd](https://en.wikipedia.org/wiki/Pure_Data).) These platforms are useful, and I use plugins written in Max4Live _every day_. Awesome stuff. Max and Pd are both visual programming languages.

Textual languages for programming music are quite different from visual languages like Max or Pd. With Max or Pd, one typically builds programs in advance, and at performance or recording time one is mainly _using_ the programs. So one "builds" the program and at performance time one _uses_ it, like an instrument. With textual livecoding environments, you have more opportunity to write the program live, and hear the audio in realtime; critically, you can practice and learn to type out code very fast, which can help keep the performance interesting.

You can bend a tool to your will, but more often, the tool guides your hand. Sure, you _can_ improvise writing Max programs, you _can_ meticulously sculpt programs in Sonic Pi. But tools lend themselves to certain styles of playing. And the _livecoding_ style is intriguing.

> Live coding [...] is a performing arts form and a creativity technique centred upon the use of improvised interactive programming. Live coding is often used to create sound and image based digital media, as well as light systems, dance and poetry, though is particularly prevalent in computer music, combining algorithmic composition with improvisation. Typically, the process of writing is made visible by projecting the computer screen in the audience space, with ways of visualising the code an area of active research. [[Wikipedia: "Live coding"]](https://en.wikipedia.org/wiki/Live_coding)

Personally, I'm not trying to perform pure livecode sets, but rather, learn livecoding as another instrument. You can get very fast at iterating and experimenting with text-livecoding. I'm interested in it as a studio tool, and a way to jam with friends. As a studio tool: because each interface has its own constraints, and constraints can inspire creativity (since "You can't have art without resistance in the material" — William Morris). To jam with friends: because it's fun!

## Get fascinated with a couple music livecoding videos

You can see a whole bunch here, [TOPLAP.org](http://toplap.org/); or here are a couple highlights:

* Sonic Pi:
  * [a bitta dub techno](https://www.youtube.com/watch?v=a1RxpJkvqpY)
  * [some ambient](https://www.youtube.com/watch?v=5fwGHAdoaXA&index=1&list=PLCTmva6IpNvlSAAkeu_VRSgb07Nwbvz9n)
* Tidal:
  * [a promo video by yaxu, that I found easy to follow :)](https://youtu.be/au65p9oRJqI?list=PLCTmva6IpNvlSAAkeu_VRSgb07Nwbvz9n&t=125)
  * [more yaxu](https://youtu.be/FenTeBMkAsQ?list=PLCTmva6IpNvlSAAkeu_VRSgb07Nwbvz9n&t=186)

Or for a very broad perspective, seek out stuff on [toplap wiki: "Videos, Articles and Papers"](http://toplap.org/wiki/Videos,_Articles_and_Papers)

## My recommendations

I suggest you try Sonic Pi first. Here's info on Sonic Pi and some other items, to help you break into this interesting world.

Here's an introduction that doesn't cover _everything_, but covers my personal interests. Filtering down for you so hopefully you don't get overwhelmed.

0. For instant gratification, check out [TinyRave](http://tinyrave.com/tracks/47-maple-leaf-rag), a pure-JS livecoding environment, with a website to field contributions. Runs in your browser!
0. [SuperCollider](http://supercollider.github.io/) "is an environment and programming language originally released in 1996 by James McCartney for real-time audio synthesis and algorithmic composition" ([Wikipedia: "SuperCollider"](https://en.wikipedia.org/wiki/SuperCollider)). SuperCollider comprises a realtime audio engine (server) and a C-like client language (client). Sonic Pi and Overtone are two popular clients these days. I didn't like the SuperCollider client language so much, so I moved onto Sonic Pi ...
1. **[Sonic Pi](http://sonic-pi.net/).** It's a different client language for the SuperCollider engine (plus some stuff, like some useful synth presets). The language is inspired by Ruby and Python. [You can put Sonic Pi on a Raspberry Pi](https://www.raspberrypi.org/documentation/usage/sonic-pi/), making it a great project for classrooms etc. It's easy to pick up, but [it's not just a toy.](https://github.com/josephwilk/sonic-pi-examples) Created and mainly maintained by [Sam Aaron, who you can see presenting on it](https://www.youtube.com/watch?v=ENfyOndcvP0).
2. If/when you want to try something else ...
  1. [Overtone](http://overtone.github.io/). Clojure client. Also uses SuperCollider. Quite popular. I haven't tried it yet.
  2. [Tidal](http://tidalcycles.org/). Haskell DSL. Less popular, yet very compelling. It's weird. It focuses on patterns and rhythms.
      1. According to the official [homepage](http://tidal.lurk.org): "Tidal is a language for live coding pattern(s). It provides a way to express music with very flexible timing, providing a little language for describing patterns as discrete sequences (which can be polyphonic and polymetric), some generators of continuous patterns (e.g. sinewaves, sawtooths) and a wide range of pattern transformations."
      2. [The paper about it, by creator Alex McLean (yaxu)](https://raw.githubusercontent.com/yaxu/Tidal/master/doc/farm/farm.pdf)
      3. Tidal can be hard to install, so at first, you may want to use [this Docker image](https://github.com/DoubleDensity/tidebox) (or [this fork, which is set up for MIDI rather than audio](https://github.com/lvm/tida1vm))

How I think of Sonic Pi vs. Tidal for my needs

* Sonic Pi for a more malleable thing (easier for me to pick up and be intentional about) (but [it's not a toy!](https://github.com/hangtwenty/dadaconf-livecoding-guide/issues/1)
* Tidal for GETTIN' WEIRD and making cool drum patterns (more surprises)

## More resources

* Overviews, communities...
  * [TOPLAP has a great introduction to livecoding overall.](http://toplap.org/about/) Just don't get overwhelmed by how many choices there are :) The key is to Just Pick Something and Start Playing.
  * [Joseph Wilk, "Live Coding - Repl Electric," an exuberant tour of a few things](http://blog.josephwilk.net/art/live-coding-repl-electric.html)
  * [Wikipedia: "Live coding" for that encyclopedic perspective](https://en.wikipedia.org/wiki/Live_coding)
  * [Join TOPLAP on Slack](http://toplap.org/toplap-on-slack/): good community, also you can just learn a lot by being a fly on the wall
  * [Various more environments shouted out in this HN thread](https://news.ycombinator.com/item?id=11054319).
* Max/MSP and Pure Data ... _not textual_ like many of these other things, though
  * [The difference between Max and Pd](https://puredata.info/docs/faq/pdmaxjmax)
  * I prefer Max/MSP because of integration with Ableton Live via [Max4Live](https://www.ableton.com/en/live/max-for-live/)
  * PureData is open-source and truly free
* Browser-based (mainly these are just novelties ... not fully capable)
  * [musiclab.chromeexperiments.com](https://musiclab.chromeexperiments.com/Experiments)
  * [TinyRave](http://tinyrave.com/tracks/47-maple-leaf-rag)
  * [studio.substack.net](http://studio.substack.net/-/recent) (TURN YOUR SPEAKERS DOWN)
* You can put Sonic Pi on a Raspberry Pi. You can also do [other audio stuff](https://www.raspberrypi.org/blog/pi-synthesisers/)
* Supercollider & Sonic Pi
  * ["Aerodynamic" by Daft Punk: tutorial to recreate it in Sonic Pi](https://aimxhaisse.com/aerodynamic-en.html)
  * [sc140](http://supercollider.github.io/community/sc140), basically "Supercollider Golf," a series of compositions in <= 140 chars of Supercollider code
* Tidal
  * [kindohm's tidal-pattern-every-day tumblr](http://365tidalpatterns.tumblr.com/) has gone past 365 now!
  * [yaxu's "patternlib" of Tidal patterns, that he released along with a recent release](http://slab.org/tmp/patternlib/)
* aaand a big ol' [list of livecoding environments](http://toplap.org/wiki/ToplapSystems)
 
----

# [Livecoding](https://en.wikipedia.org/wiki/Live_coding) to produce **visuals**

Unlike livecoding music, livecoding visuals doesn't have a non-coding/non-technical counterpart (3D modeling/animations would be the closest thing, but that's fairly technical in itself). So where do we begin?

Let's start by considering some things in a list:
* intentional results vs. play and happy accidents
* interactivity
  * with user input
  * with sound
* models/scenes vs. patterns
* construction vs. manipulation

... Okay, that was... interesting, maybe? Dull, possibly? This is just some vocabulary we'll use to discuss options.

Let's talk about technology now.

## Rendering

Technically, all computer graphics is rendering, but let's clarify what we mean when we talk about it here. Rendering is about putting geometrical data onto the screen. A line, a cube, a tree, an infinite checkerboard plane -- all this is geometric in nature.

When we want to _construct_ visuals, it's usually a good idea to reach for something with general rendering capabilities. 

Conceptually, this type of environment generally has you write programs in one of two ways:
* statefully: 
  * the program "moves" about the virtual world and sets rendering properties (color, opacity, etc) and then places geometry into the scene relative to the current state of the program
  * it's as if you're flying around this virtual world with a fancy paintbrush that you dial in some settings on and then use to draw things into existence
  * most rendering API's seem to use this model, especially if they are based on low-level API's like OpenGL
* declaratively:
  * the program consists of declarations of where in the scene various geometry exists 
    * note: there's no concept of a "current position" for the program, only for the objects that exist in the scene
  * you are describing all things in the scene independently; there is a room 12x20 with yellow walls, there is a brown couch centered along the far wall

Example (taken from [cyrilpatterns](http://cyrilpatterns.tumblr.com/post/100572666612/i-i-001-for-x-3-to-4-step-1-for-y-3-to-4)):
```
i: i + 0.01
for x: -3 to 4 step 1
  for y: -3 to 4 step 1
   push
    move x, y
    if noise(x * i, y * i) > 0.25 
     box 0.25
    end
   pop
  end
end
```

### Environments

* [livecodelab](http://livecodelab.net/play)
  * browser-based, super simple graphics and audio
  * start here if you just want to get pixels on the screen
* [gibber](http://gibber.cc/) ([docs](http://bigbadotis.gitbooks.io/gibber-user-manual/))
  * a browser-based js livecoding environment with 2D and 3D graphic support
  * you can generate audio and graphics and then map their properties to each other, such as the frequency or volume of a melody to the rotation or color of some cube
* [fluxus](http://www.pawfal.org/Software/fluxus/) ([docs](http://www.flossmanuals.net/fluxus/))
  * a game engine (i.e. does graphics, sound, user interaction) based on Racket (a lisp)
  * has [integration with DrScheme](http://en.flossmanuals.net/fluxus/ch024_fluxus-in-drscheme/) IDE

## Shaders

Technically, shading is a part of the rendering process, but we can use shaders without actually talking about geometry. Shaders are programs that run after geometry has been specified (or not) in order to take the virtual scene and determine how it is drawn on the screen. 

What makes shading different than the general "rendering" above is that a shader (usually) does not _construct_ a scene; rather, it takes a scene and position as input and outputs what would appear on the screen at that position. A cube in the scene, appears on the screen in 2D, and a shader is used to transform the cube into a 2D representation which is then drawn on the screen. 

Side-note: the fact that a shader only applies to one point on the screen at a time makes it easy to parallize, which is why they usually run on GPUs which in turn is why they are written in shader-specific languages that may have limitations that general programming languages don't.

So, in the simplest case, a shader is a very direct translation of the geometry in a scene, but they can also compute special effects, like lighting, fog, textures, etc. Or for our purposes, shaders can just make cool abstract patterns that evolve over time, possibly in response to some audio input!

### Environments

* **[The_Force](https://shawnlawson.github.io/The_Force/)** ([sourcecode](https://github.com/shawnlawson/The_Force)) -- **make sure you use HTTPS,** at the time of writing Microphone Input will only work with HTTPS. You want that!!!
  * browser-based environment for livecoding OpenGL/WebGL Fragment shaders with some cool built-in functions for integrating with audio input
  * [examples](https://github.com/shawnlawson/The_Force_Workshop)
  * [more examples](https://github.com/shawnlawson/The_Force/tree/c3d7aa28cca1fd5e7f64a5809a649d95fda9ccc1/shaderExperiments)
  * examples from dadaconf 0.1
  	* by [kevincairo](https://github.com/kevincairo): [examples](https://gist.github.com/kevincairo/40cdbc9758f546ac3a73728dce62216f)
  	* by [hangtwenty](https://github.com/hangtwenty): [examples](https://gist.github.com/hangtwenty/568cde2bf2e52f6a5c3982006ffa68ab) (sloppy)
  * **[THE BOOK OF SHADERS](http://thebookofshaders.com/)** is the most comprehensive single resource of examples around! Some examples may have different variable names and such, so these aren't just copy/paste examples. But if you want to get INTO IT and understand what you're doing, this book is your friend.
  * The_Force is great for a two person performance (one person on visuals, one on audio) (... or one human + pre-arranged audio) (... or one human, and only modifying the visuals occasionally, mainly performing audio)
* [Shadertone](https://github.com/overtone/shadertone)
  * overtone + shadertoy!
  * Sounds a lot like The_Force but since it's not browser-based, it will take some more effort to get started (which may be worth it!)
  * Has support for writing shaders in a lisp-like language, if you're into that sort of thing


### The_Force

This is the moment _I_ have been waiting for. The_Force is the funnest way to produce visuals in my experience, but there are other options that may be worth exploring depending on synergies they might have with other technologies you are using.

#### Example
Let's start playing! Just copy the following snippet into [The_Force](https://shawnlawson.github.io/The_Force/) and it should start with a static pattern. Uncomment the commented code to change the variables and see the results. Hopefully you'll start to see the way the values are interacting to bring the expected results.
```
void main () {
    // the pixel position we're drawing (relative to bottom-left, width and height range from 0.0 to 1.0)
    vec2 st = uv(); 

    // the pixel position we're drawing (in terms of some weird coordinate system, relative to center of screen)
    vec2 stN = uvN(); 
    
    vec2 pivot = vec2(.5, .5);

    float rotationAmount = 
        // time * .3; // rotate slownly over time
        0.;

    vec2 stretch = 
        // vec2(abs(sin(time * .5))*4., 1.);    // elongates the y axis
        // vec2(0.5);                       // enlarge / zoom in
        // vec2(10.);                       // shrink / zoom out
        vec2(1., 1.); 

    vec2 shift = 
        // vec2(0., -time);             // pattern moves along -y axis (up, weird i know)
        // vec2(cos(time), sin(time));  // shifts around in a circle
        vec2(0., 0.);

    vec3 color = 
        // orange + sin(time) * teal; // evolves between orange and orange + teal
        teal;

    vec2 pixelate = 
        // vec2(500000.); // don't know why this works
        vec2(0.);

    // This is a pattern that will get drawn, all the variables above affect how it turns out!
    vec3 f = color + snoise(
        rotate(pivot, st, rotationAmount) 
            * stretch 
            + shift 
            + pixelate);
    
    vec3 g = 
        // voronoi(rotate(pivot, st, rotationAmount * .5) * vec2(10.)) + red;   // just some weird stuff!
        // texture2D(backbuffer,  st).rgb;                                      // value in previously drawn frame, distorted from a coordinate transformation
        texture2D(backbuffer,  stN).rgb;                                        // value in previously drawn frame
    
    float fgRatio = 
        // .25 + (sin(time) * .5); // fade between f and g
        .5;
    
    // output the fragment result, a blend of f and g
	gl_FragColor = vec4(mix(f, g, fgRatio), 1.0);
}
```

If you are having fun, great! If you sort of get what's happening even better! If it doesn't seem to make any sense, don't worry -- we can still have fun as long as we can piece together a valid program, even if it's random nonsense.

#### Interacting with audio.

This is my favorite part. The_Force allows you to channel in audio and then interact with it through some built-in variables.

First, let's grab a soundcloud track url and go to the bottom of The_Force and click the mic. Go to the soundcloud tab and paste the url and hit load. Sound!

Now, let's react to it! The `bands` variable is a built-in `vec4` variable which is defined by the levels of the FFT of the incoming audio. In other words:
* `bands.w` is the level of the low frequencies
* `bands.x` is the level of the mid-low frequencies
* `bands.y` is the level of the mid-high frequencies
* `bands.z` is the level of the high frequencies

We can then plug any of these components into the place of a `float` value in the program! For example, try replacing the `fgRatio` value with something like `bands.w` to make the `g` pattern pulse in on the bass thump!

You can use microphone input too :)

#### Lastly ...

If you do get into playing with shaders, don't forget **[The Book of Shaders](http://thebookofshaders.com/)**!
