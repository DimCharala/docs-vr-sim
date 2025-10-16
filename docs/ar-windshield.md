# AR Windshield

This is the main feature of the application. It is a 100x24cm screen in front of the driver which displays important information for the safety of the driver.

![The AR Display inside the Simulation](assets/ar-windshield-description.png)

## Display Features

* [AI Cars](ai-cars.md) and Pedestrians
* Traffic Warnings
* Obstacle Warnings

## How it works

This feature works using two different mechanics. It uses [Post Process Materials](https://dev.epicgames.com/documentation/en-us/unreal-engine/post-process-materials-in-unreal-engine) and Unreal Engine's [Scene Capture Components](https://dev.epicgames.com/documentation/en-us/unreal-engine/1.7---scene-capture-2d?application_version=4.27).
Specifically for the visualization of the danger levels of Cars and Pedestrians only Post Process Materials are needed, which use the depth buffer and Unreal Engine's [Custom Depth Buffer](https://www.tomlooman.com/the-many-uses-of-custom-depth-in-unreal-4/), which is basically a depth buffer only for selected actors in the scene.

## Details

!!! note "AI Cars and Pedestrians"

    The AI Cars and the Pedestrians are explained in more detail on their own page [here](ai-cars.md).

### Traffic Warnings

![Forbidden traffic sign during traffic light](assets/traffic-warning-forbidden.png)

While driving the user has to pay attention to the traffic laws and to traffic sign indications. Using instances of these signs to inform and warn the driver for potential speed limits, stop warnings or traffic lights. The position of these warnings is static, so the position of these should be manually placed or spawned using an external server with the information (and potentially websockets).

### Obstacle Warnings

![Dip warning](assets/dip-warning.png)

This part refers mainly to static obstacles, like dips or bumps in the road. Using the same logic as with the traffic warnings, which is that the position of these should be manually places or spawned using an external server with information, they warn the driver about the obstacle and visualize the general area of the obstacle. As an example the dips require a radius of it (or at least an estimate) to visualize it using a circular warning on the ground.

## Next steps

* Fixing position of projected elements on VR
* Adding more traffic signs
* Connecting with data base



