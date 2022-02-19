Custom NPC Outfits is a Stardew mod that allows players and creators to readily customize NPCs using the power of Content Patcher.

## How it Works
Custom NPC Outfits works by seperating an NPC's sprite into many pieces, refered to here as layers, and then dynamically building 
their portraits and sprite sheets from those assets. This provides the ability to deeply customize the appearance of NPCS, 
from their hairstyles and outfits to their accessories.

These layers load in this order (Note that not all NPCs have all of thes layers):
- **Base** -- The base body sprite
- **Hair Underlayer** -- The back layer for hairstyles, which goes behind the head and clothing.
- **Bottom Layer** -- The bottom layer for tops. THings like undershirts, tank tops, and similar.
- **Legs** -- Pants and shorts -- character sprites only.
- **Middle Layer** -- Jackets and overclothes
- **Neck Accessories** -- Necklaces, chokers, scarves, and similar accessories.
- **Hair Front Layer** -- The front layer for an NPC's hair, which overlaps all clothing.
- **Hair Accessories** -- Hairclips, hats, and other accessories that go on the head.
- **Overlayer** -- Layers of decoration over the top of a sprite, such as hands or emotes.

Not all of these layers are currently implemented.

## Clothing Classes
Because of the vareity of clothing that exitst for characters, one ease of use tool that Custom NPC Outfits provides is clothing classes,
which act as the general groups of clothing that a person might wear. This also allows Conent Patcher to distingush
clothing types by weather and season, giving deeper customizability to the system.
Each NPC has their own predifined clothing classes, but adding more only requires the adjustment of the NPC's clothing handlers.

## Adding your own Assets
WIP
