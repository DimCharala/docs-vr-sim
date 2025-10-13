# AR Windshield

This is the main feature of the application. It is a 100x24cm screen in front of the driver which displays important information for the safety of the driver.

![The AR Display inside the Simulation](assets/ar-windshield-description.png)

## Display Features

* [AI Cars](content-tabs.md) and Pedestrians
* Traffic Warnings
* Obstacle Warnings

## How it works

This feature works using two different mechanics. It uses [Post Process Materials](https://dev.epicgames.com/documentation/en-us/unreal-engine/post-process-materials-in-unreal-engine) and Unreal Engine's [Scene Capture Components](https://dev.epicgames.com/documentation/en-us/unreal-engine/1.7---scene-capture-2d?application_version=4.27).
Specifically for the visualization of the danger levels of Cars and Pedestrians only Post Process Materials are needed, which use the depth buffer and Unreal Engine's [Custom Depth Buffer](https://www.tomlooman.com/the-many-uses-of-custom-depth-in-unreal-4/), which is basically a depth buffer only for selected actors in the scene.



## Next additions

TBD


