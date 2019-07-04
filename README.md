# quadrophenia
Quadrophenia (Three.js project)

John Linnane
118227214
MSc Interactive Media
2018/2019

Web XR Assignment: ‘Quadrophenia: A Tour of UCC’s Quad’

********************************************************************

This assignment uses the WebGL renderer and the Three.js library to create an immersive tour of UCC’s quad, through the lens of a hellish version of 1979’s Quadrophenia movie.

For image textures I textured a projection of a movie on a large billboard behind the quad, I also textured a large cube to the left of the quad. For normal mapping I used an image of a stone ground texture, along with it’s normal map, to give the impression of depth. For environment mapping I created a ‘sky box’ cube large enough to surround the whole scene, this was textured with an image of red clouds.

I loaded various external objects into the scene using a combination of GLTFLoader, OBJLoader and Colladaloader. These objects had shadowing enabled.

I used a vertex shader and a combination of three different fragment shaders to make the three bollards along the front of the quad.

For a soundtrack, the song My Generation is played automatically when the scene is loaded.

I used a combination light types in my scene, including Ambient and Spotlight. The spotlight in the foreground has animated movement, intensity, colour changes and eventually switches off.  The system changes resulting from the light change events are printed to the console. Another light follows the moving scooter as it comes around the right side of the quad.

I used the WebGL renderer to enable headset capabilities. Line 176 of the html file should be uncommented to enable this feature.

For spatial sound I used the Web Audio API through the Three.js PositionalAudio class to locate motorbike engine sounds in the same position as a circling motorbike, as the user moves around the object, the sound direction changes to match the object’s position.

