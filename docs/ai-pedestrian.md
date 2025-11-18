# AI Pedestrians

The pedestrians in the current version, as of November 10th 2025, of the application use the default mannequin models. They use a simple AI Controller, which uses two states, and their goal is to reach a random target point inside the map.

## Actions

These are the main functions of each car in more detail.

### Pedestrian States

The pedestrians currently have only two states, which are Moving and Waiting. Most of the time, the moving state is used in order to reach the target point in the map. However the pedestrians need to wait for the traffic lights. In that case the waiting state is used until the traffic light allows the pedestrians to cross it.

### Target Points

There are multiple random points inside the map, which are assigned randomly at the start of the simulation or when a pedestrian reaches one. These serve as the goal of the pedestrians which they try to reach.

## Next steps

These are next addition to the project. Any step that is completed will be struck through ({--example--}).

* Custom low poly pedestrian models (currently using some free ones, may stick with them)
* More complex movement
* Fix traffic light bugs
* Spawning/despawning for more realism near the player