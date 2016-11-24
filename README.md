# rn-sprite

rn-sprite is a react native component for creating `animations` from `spritesheets` for IOS and Android devices


##### ...Spritesheets? ...Animations?
A `sprite` is a single graphic image that is incorporated into a larger scene so that it appears to be part of the scene.
When you put many sprites into a single image, you get a `spritesheet` like [this][h-sprite] and [this][v-sprite].
The process of changing images in quick succession to give the illusion of movement is called `animation`.

<img src="https://github.com/adhbh/rn-sprite/raw/master/demo1.gif" width="200"> <img src="https://github.com/adhbh/rn-sprite/raw/master/demo2.gif" width="200">



  - Depends on [gl-react-native][gl-rn]
  - Works on IOS and Android
  - Supports both [horizontal][h-sprite] and [vertical][v-sprite] spritesheets
  - Play/Pause support
  - Configurable animation speed
  - Touch responsive

### props
| prop | type | description | required |
|------|------|-------------|----------|
| **source** | string | Url of spritesheet image | yes |
| **sequence** | array | Array of numbers between 0 and 1 that define the sequence of animation | yes |
| **loop** | boolean | Repeat the animation when it completes (Default: `true`) | no |
| **fps** | integer | Frames per second (Default: `2`) | no |
| **isPlaying** | boolean | Play/Pause the animation (Default: `true`) | no |
| **onTouchStart** | function | Function which is called when sprite is touched | no |
| **onTouchMove** | function | Function which is called while the user touches and moves the finger on the sprite | no |
| **onTouchEnd** | function | Function which is called when touch event gets completed | no |

### Usage
- Animations in mobile games
- Replacement for `gifs`
- 360-View

### Todo
- Configurable repeat count for animation
- Rewind support
- Got some more ideas? Feel free to raise a PR

License
----
MIT


   [gl-rn]: <https://github.com/ProjectSeptemberInc/gl-react-native>
   [v-sprite]: <http://assets.myntassets.com/assets/360images/1481063/FILA-Men-Navy-Epifanio-Sneakers-4881474692323372-1481063_360.jpg>
   [h-sprite]: <https://cdn.codeandweb.com/blog/2014/11/05/animate-sprites-in-css-with-texturepacker/capguy-walk.png>
