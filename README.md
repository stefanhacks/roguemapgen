<p align="center">
  <img src="https://github.com/user-attachments/assets/fd4a5c58-9a14-4f27-b53e-a361fba9f18f" />
</p>

# Roguelike Map Generator in Godot

### Room algo works by:
- Slices the screen in nine zones with variable horizontal and vertical sizes.
- Merges one to three cells.
- Randomizes horizontal lines which contain no merges.
- Cuts out some of the areas for variety.
- Creates a square room of variable size and point inside each space.
- Possibly adds extra walls to each corner of each room to make it look a bit more organic.

### Pathways generated by:
- Shuffles the list of rooms.
- Selects two random rooms.
- Selects if pathway is going to be a simple corner or a have a short lengthy segment in between.
- Selects a random spot within both rooms, within the center axis which is perpendicular to path, ensuring there's a tile there.
- Draws a line between both spots.
- Has a method which connects all rooms by iterating through a shuffled list. This ensures all rooms are connected at least once.

### Graphics:
- Used [monogram](https://datagoblin.itch.io/monogram) as the UI font.
- Original Tileset got from [Pìxel Poem, on itch.io](https://pixel-poem.itch.io/dungeon-assetpuck).
- In order to understand Godot Tileset terrains, I had to change a bit and expand in some of its options.

### Where to Go:
- Comment the code.
- Might make this prettier by adding custom rooms, objects and random objects within.
- Define navigation zones, add agents.
