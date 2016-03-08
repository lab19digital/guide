Assets should also be configured in a friendly manner:

1. If retina images are required, export these with file names as follows image@2x.png, letting the developer know that this is a retina image.
2. Also include the dimensions in the image name. E.g. 200x300-filename.png, 200x300-filename@2x.png. This is useful information that can be instantly gleaned from looking at the filesystem.
3. PNGs can include transparent space. If you export an image with transparent bleed, don't expect that it will render without this. It will render with the space as part of the image and could therefore affect the layout. 
4. Roll icons into a font icon where possible (it will require the source is in vector). Otherwise, negotiate with the designer for an icon font pack to use.