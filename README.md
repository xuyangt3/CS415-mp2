# Design document

The design consists of 4 islands. The first and third island contain only laser shooters and pursuers. The second island only have mortars. The fourth island contains a mortar and a two laser shooters.

![](img/levels.jpg)

Laser shooter is chosen as the custom enemy type because I want to restrict the player's capability to fly. Otherwise, the player could just bypass any level design and go directly toward the destination. The weaknesses of the laser shooter are:
1. The laser must be in continuous contact with the player in order to cause damage. The rate is set to once per 2 seconds of continuous contact.
2. The laser shooter's head is large, so it could be easily killed at close distance.
3. The shooter doesn't rotate very fast and have a limited (but configurable) field of reception.

![](img/laser_shooter.jpg)

The first island makes use of these features of the laser shooter. The player is supposed to move in a spiral path in order to avoid the beams. The player should separate the time of exposure under the beam among different laser shooters. The laser shooters also make it too dangerous to fly. The walls around one shooter form a safe area. After killing the laser shooter within the walls, no enemy can attack a player in the walls.

The second island is intended for the player to pass through as quickly as possible. It separates the first island and the last two islands, so they don't interfere with each other. Therefore, this level is filled with mortars. A little bit of luck is also needed to pass this level, so the player needs to try multiple times.

The third island has more pursuers than the first one. It also have laser beams from the fourth island and occasional cannon balls from the second island. The enemies from other islands are harder to reach from the player, so difficulty is increased.

The final island is where the destination is located. The two laser shooters are for the third island. The mortar is placed in front of the laser shooters to make them harder to reach. The upper half of these two laser shooters' field of view is blocked using pillars. Otherwise, they will shoot the player down when the player is jumping from the second island to the third island.

In all levels, the player needs to clear the enemies in order to safely collect the collectible and the health pack.
