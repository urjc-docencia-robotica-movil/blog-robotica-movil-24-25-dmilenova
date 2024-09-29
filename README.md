# P1 - Vacuum Cleaner
## Concept

The first solution was approached trying to simplify as much as possible, meaning that only the bumper was used to create a vacuum cleaner that tackles the task simply. Therefore the first idea is to create a vacuum cleaner that approaches the cleaning task in the following way, first it goes forward and when it hits something it goes backwards to give room for maneuver and then turns 90 degrees. This way we almost go from wall to wall and guarantee good coverage of the space and fewer collisions in the same place.

## Algorithm

The vacuum cleaner starts in the "Foward" state going foward, and remains in the foward state until the bumper detects a collision. Next when obstacle is detected the vacuum cleaner goes back so that it can turn smoothly, there for the robot goes backwards then it changes state.The next state is "Turn" in which the vacuum cleaner turns almost 90 degrees , this optimises the space that is being coverd add garanties les repetetive collisions.

## State diagram
State diagram:

![State diagram](state_diagram.png "State diagram")


## Exploration
Vacuum cleaner exploration's image after 1 hour when it finisht cleaning:

![Vacuum cleaner image](Primera_solucion.png "Vacuum cleaner image")


Video while cleaning:

![Vacuum cleaner video 1](VIdeo-vacuum.webm "Vacuum cleaner video 1")

Video towards the end of the cleaning:

![Vacuum cleaner video 2](Video_vacuum_end.webm "Vacuum cleaner video 2")

The rest of the videos:

![Vacuum cleaner video](https://github.com/urjc-docencia-robotica-movil/p1-vacuum-cleaner-24-25-dmilenova/tree/main/videos "Vacuum cleaner video")

## Difficulties

The first difficulty was that I also wanted to add the laser to be able to detect the objects before the collision, but when the laser was empty there were difficulties in continuing with the other states, that's why I decided to simplify it. Since the idea could be recreated with the bumper, it was approached like that. But when trying to create it with the bumper, there were difficulties with the "Backward" state because when entering it and then going to the "Turn" state it was already detected that there was no obstacle, that's why only 2 states were made and the starting part back was added to when the crash was detected. Later there were complications with the vacuum cleaner getting stuck in the same place, but this could be solved by increasing its angular speed and thus making it rotate more widely (90 degrees).
