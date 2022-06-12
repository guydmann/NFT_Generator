NFT and metadata generator created by NuclearGeek

[Twitter](https://twitter.com/NuclearGeekETH)

Create your own NFT collection using python

Copy the repository to your local drive

You should be able to just install missing dependencies with pip and run generate.py to generate your first collection of Framed Eyes made by NuclearGeek.

To create a custom collection:

Add your image layers to the layers folder. You can create as many subfolders as you want. 

Make sure each file name has a decimal weight after the #. This sets the rarity weight of the layer.

The layer filenames should look like this: metal#0.1.png. This would have a 10% chance of showing up. The total weight in each folder from all the images in that folder need to add up to 1.

You can use transparent layers too, just add them in the appropriate folder.

Set the number of NFTs you want to create in line 23 for max_nfts. Set num on line 22 to the starting number you want. I like 0 but some people use 1. You can change it to any number to add to a collection as well.

This script will also create metadata for your collection. The folder names will be the trait type and the layer name before the # will be the value of the trait type. 

There is a check to ensure duplicates are not created so every NFT is unique. If you keep seeing "combination exists" in your console then you might not have enough variety in your layers to create as many NFTs as you are tyring to.

You will need to append the "image" location in each json for your final collection if you want to mint it. 

Use append_json.py to update your metadata with the image uri for your collection.

Optional:

Use removeJSONending.py to remove the .json file extension if you only want data files and not json. I would recommend backing up the .json files before doing this.
copy/paste removeJSONending.py to your folder with your json metadata and run removeJSONending.py to remove .json from all files in the folder.

Use rename.py to rename or renumber files in a folder. This is helpful if you are trying to combine images you create or have to make edits.

Use giffer.py to create a gif of the images you create.

Use collage.py to create a collage of images. Place images in the collage folder and run collage.py to generate the image. You can adjust width, height, and row for size and number of images you want. 

Have Fun! 

