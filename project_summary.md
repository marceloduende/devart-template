# Project Title
Kubricks Cube, the rubiks cube with style.

## Authors
- Marcelo Duende, marceloduende

## Description
The idea was to push my math skills. Everyone knows how hard is to figure out the pattern to solve the Rubik's Cube. So I decided to build a solvable Rubik's Cube. I am not concerned about how the tech boundaries are being pushed to the next level, all I am looking for is to have fun. If my fun time pushes technology to the next level, well, then I am a happy winner.

## Link to Prototype
[Kubrick's Cube](http://kubrickscu.be/ "Kubrick's Cube")

## Example Code
NOTE: Wrap your code blocks or any code citation by using ``` like the example below.
```
/******************** ADD AND POSITION CUBES ON THE 3D SPACE *******************/
function addCubes(){
	for(var x_loc = 0; x_loc < 3; x_loc++) {
		for(var y_loc = 0; y_loc < 3; y_loc++) {
			for(var z_loc = 0; z_loc < 3; z_loc++) {
				cube = kubricks.cube(x_loc, y_loc, z_loc);
				cube.position.x = (x_loc - 1)*(cube_size + gap_between_cubes);
				cube.position.y = (y_loc - 1)*(cube_size + gap_between_cubes);
				cube.position.z = (z_loc - 1)*(cube_size + gap_between_cubes);
				cube_wrappers.push(new cube_wrapper(x_loc, y_loc, z_loc, cube));
				scene.add(cube);
				objects.push(cube);
			}
		}
	}
	
}
```
## Links to External Libraries
 NOTE: You can also use this space to link to external libraries or Github repositories you used on your project.

[Example Link](http://www.google.com "Example Link")

## Images & Videos
NOTE: For additional images you can either use a relative link to an image on this repo or an absolute link to an externally hosted image.

![Example Image](project_images/cover.jpg?raw=true "Example Image")

https://www.youtube.com/watch?v=30yGOxJJ2PQ
