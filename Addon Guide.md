This guide provides information on adding new assets to **Dynamic Character Portraits**.
As I add new functionality, I will add more tutorials.

## Overview
Every character has the following asset groups:
* Hair, seperated into front and back parts.
* Clothing, seperated into two (or more) layers and then into Clothing Groups
* Accessories of various groups
* Body assets, which are base assets such as the face and any emotes, as well as a template torso for creating your own assets.

## Adding an asset
This include things like accessories or pieces of clothing for already-defined clothing types. 
It can also include hair assets, but depending on the character it may require you to have a front and back asset.
Assets should always be in PNG format.

Most assets have a fairly strict naming convention:
* Hair: Hair_#.png (For both front and back pieces)
* Clothing: (clothing_type)_#.png

Accessories don't have strict naming conventions.
When looking for the matching tokens for characters, be sure to look at the comments, 
and not the names of the tokens.

### Accessories
* Add the asset to the appropriate accessory folder
* Locate the matching dynamic token for that character and accessory in the content.json
* Add the name (minus the file exension) to the values.

### Hair
* Add front and back hair assets to the appropriate folders (Located in Character/Hair)
* Locate the hair dynamic token for that character in the content.json
* Add the # (asset number) to the values.

### Clothing
* Add clothing assets to the appropriate folders (Located in Character/Clothing)
* Locate the matching dynamic token for that character in the content.json
	 * Tip: Check the When arguments of statements for this, or use the comments. It's not as obvious as for hair and accessories.
* Add the # (asset number) to the values.

## Adding a Clothing Group
Adding a new clothing group is slightly more complex, but allows you to define new types of clothing.
This is mostly useful for organization now, but will later allow the plugin to choose clothing types based on season, weather, etc.
Remember, all assets within a clothing type should be named as follows: `(clothing_type)_#.png`

* Add a new folder in the appropriate Clothing/Layer (either Bottom Layer or Top Layer)
* Add assets  for new clothing type to this folder.
* Find the appropriate layer token in the content.json, and add the name of the new clothing type to the Random values.
* Add a new version of the related selector, with the When argument looking for your new clothing type.
* Add the # (asset numbers) to the Values argument, as normal.

## Swapping Portrait Sets
This is not currently implemented, and likely won't be for a while; once it is, I'll leave a walkthrough here.
However, it should be a simple affair, involving using Config Schema and some minor alterations to the file directory structure.