![Pic](https://user-images.githubusercontent.com/57761255/110940257-a7703f00-8347-11eb-9e10-66e91c07c910.png)

Let's say you made a map and now you need to add gaming zones.

## How to open a map in TeeUniverse Editor

- Choose `File` -> `Import Teeworlds Map` -> `TeeWorlds Maps` (or `TeeWorlds Downloaded Maps`) -> `Open`


## Add infclass packages

For drawing zones and curved warning, tapes need to open 2 packages 'infclass' and 'env_infclass'.

- Choose `File` -> `Open Package` -> `Global packages` -> `infclass` (or `env_infclass`) -> `Open`


## Drawing the zones (logic)

Group Zones is on the left bottom panel.


![Zones in editor](https://user-images.githubusercontent.com/57761255/110866489-40ff0880-82d6-11eb-9a34-58db4a810903.png)


There are 2 ways to draw a zone — by tiles or freeform in TeeUniverse.

### Zone by tiles

1. `Zones` -> `Add Zone Tile Layer`. 
2. On the right panel: name the zone 'Infected zone' (or 'Bonus zone' )

![Name of zone](https://user-images.githubusercontent.com/57761255/110868760-38103600-82da-11eb-8aa0-a85d786cff01.png)

3. On this panel choose a type of zone:
- `icDamage` - death zone,
- `icBonus` - bonus zone,
- `icTele` - zone forbidding teleportation for scientists or spawning zombies by a witch)

4. Press SPACE to select the zone subtype.

For death zone:

![изображение](https://user-images.githubusercontent.com/57761255/110869931-8292b200-82dc-11eb-89c7-843b7b576302.png)

For bonus zone:

![Subtypes of death zone](https://user-images.githubusercontent.com/57761255/110870097-d8675a00-82dc-11eb-81c9-f6ec1c9beec1.png)

There are hints for each subtype on the top of the view.

5. Draw the zone.

![Subtypes of bonus zone](https://user-images.githubusercontent.com/57761255/110870689-05683c80-82de-11eb-9ba2-7ccfeccb1dc8.png)

6. Drawing tools.

![Tools](https://user-images.githubusercontent.com/57761255/110870870-60019880-82de-11eb-8913-57dffb4463ad.png)

For drawing use the `Stamp Tool`. Description of each tool at the bottom right.

### Freeform zone

1. Zones -> `Add Zone Object Layer`. 
2. See `p2` at [Zone by tiles](#zone-by-tiles).
3. See `p3` at [Zone by tiles](#zone-by-tiles).
4. Select `Line Drawer` tool and draw closed polygon.
 
![Tools](https://user-images.githubusercontent.com/57761255/110885420-e080c300-82f7-11eb-8d99-1de3aa49b7e7.png)

![Figures](https://user-images.githubusercontent.com/57761255/110873121-1c109280-82e2-11eb-8772-3e2496b75c7f.png)


5. Press '+' or '-' to select a subtype of the zone on the right bottom panel.
 
![Selector of subtype](https://user-images.githubusercontent.com/57761255/110872475-f040dd00-82e0-11eb-8672-2d4536f0c47d.png)

6. Select the `Vertex Editor` tool to adjust (fix the position) of the polygon vertices.


## Decorate zones (tapes and filling)

1. On the left bottom panel choose `Background Layers` -> `Add Background Group`.

![Background Layers](https://user-images.githubusercontent.com/57761255/110874181-5e3ad380-82e4-11eb-84e7-b4406aed69de.png)

2. Name the group according to the zone ('Infection Zone' or 'Bonus Zone').

### Tapes

1. Select the created group -> `Add Object Layer`.
2. See `p2` at [Zone by tiles](#zone-by-tiles).
3. Select `Line Drawer` tool and draw a line (tape).
4. Select a style of tape (`warnLine` or `bonusLine`) on the right bottom panel

![Styles selector](https://user-images.githubusercontent.com/57761255/110875334-7a3f7480-82e6-11eb-866c-dc9d28dcfcaf.png)

![Image of tape](https://user-images.githubusercontent.com/57761255/110875391-93e0bc00-82e6-11eb-89ab-bcd0086b8f71.png)

5. Select `Vertex Editor` tool to align (fix the position) of the line vertices.
6. If you want to change the line shape, select a point and choose `Smoothness type` on the right panel (use `Vertex Editor` tool).
For round the vertices of line select `Automatic` Smoothness type.

![Smoothness type](https://user-images.githubusercontent.com/57761255/110876348-5715c480-82e8-11eb-9650-b4ad530995e2.png)

![Tapes](https://user-images.githubusercontent.com/57761255/110876559-c986a480-82e8-11eb-8b32-159f55094611.png)

### Zone (visible part)

#### Bonus Zone

1. Select the 'Bonus Zone' group -> `Add Object Layer`.
2. Name an object.
3. Draw a polygon inside of the tape.
4. Select the object on the right panel and choose the style

![Style](https://user-images.githubusercontent.com/57761255/110879158-87ac2d00-82ed-11eb-9ad9-6d77d272b75c.png)

You will see a purple area inside the tape

![Bonus area](https://user-images.githubusercontent.com/57761255/110879284-c346f700-82ed-11eb-9b95-f36ec8179d31.png)

#### Infected Zone

There is no infected zone in TeeUniverse and you will have to create it yourself.

1. Select `Edit` -> `New Path Material`

![Edit](https://user-images.githubusercontent.com/57761255/110879485-22a50700-82ee-11eb-8d8d-43a55100988d.png)

2. Name the part
3. Select `Filling Enabled`
4. Select a circle figure on the top of the view

![Circle](https://user-images.githubusercontent.com/57761255/110879712-7fa0bd00-82ee-11eb-8056-c644a0a29a1a.png)

5. Choose `Texture Color` and set values like on the picture

![Texture Color](https://user-images.githubusercontent.com/57761255/110880160-38ff9280-82ef-11eb-9935-1e8703976f4d.png)

6. See `p1-p4` at [Bonus Zone](#bonus-zone).

![Bonus Zone](https://user-images.githubusercontent.com/57761255/110880743-25a0f700-82f0-11eb-8482-143a3a17790c.png)

### Zones Items

![Zones Items](https://user-images.githubusercontent.com/57761255/110880933-79abdb80-82f0-11eb-9df6-96cd101c95cd.png)

1. Select the created group ('Infection Zone' or 'Bonus Zone') -> `Add Quad Layer`.
2. Name a layer and select 'Infclass' image on the right panel

![Images selector](https://user-images.githubusercontent.com/57761255/110881185-fb9c0480-82f0-11eb-85c1-0cbc522e5ac6.png)

3. Select Stamp Tool and press SPACE to select tiles.


## Spawn and Flags

1. `Entities` -> `spawns` or `flags`
2. Press SPACE and choose spawnpoints or flags

![Spawnpoint and flags](https://user-images.githubusercontent.com/57761255/110882559-30a95680-82f3-11eb-8802-4661f14e4aa3.png)

3. Add spawnpoints or flags to the map using the grid alignment (so they don't hang in the air)

![Flag on map](https://user-images.githubusercontent.com/57761255/110885267-9992cd80-82f7-11eb-9243-08b2ae76980b.png)

Note: It is recommended to use a separate entity group for flags.

## How to save the map

- Choose `File` -> `Save package as` -> `Home` -> Your Folder

