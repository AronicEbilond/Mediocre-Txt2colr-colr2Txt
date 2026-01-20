# Mediocre-Txt2colr-colr2Txt
A basic text to color, color to text converter. Made it with AI. Wish I could make it myself, but I don't know how to program nor where to start.

The pixels themselves will be organised like they are in the image, but in text, like character-art, you know?
Same goes for the modifier-document for more complex colors & mixed colors.

Basic Overview of what characters mean what;
ROYGCBIVPM PLUS N, W, G, lowercase letters, b letters for their corresponding colors(capital N is for noire which is black in english by the way, so that's why its not the same. Lowercase b is for brown btw);
Red,
Orange,
Yellow,
Green,
Cyan,
Blue,
Indigo,
Violet,
Pink,
Magenta,
Black,
White,
Gray,
brown,

We will have another layer of code in a seperate text file, for different shades of these colors and for these colors too, with this layer distinguished as modifying the pixels it does, via the positioning in the text file, indicated via comas.
So, for example, 101, would be considered at column 1 and row 1, and the one following it, will be interpreted as being at column 2 row one, with it working via deeming the position based on what it'd look like if there were only comas, with the numbers used for telling the program what the color-modifier will be, and the coma, being used, after interpreting what the positioning of the numbers in the document would look like, with only comas in the document, because that is valueble position data...
Edit: Ontop of the existing modifier-layer, we will have a cleaning-layer, for fixing oddly patched pixel areas that lack smooth transitions between one area of pixels to another, i.e. brown pixels to pink pixels, due to the smoothness being lost in conversion due to data being necessarily simplified, to create the "ROYGCBIVPM+NWGb" channel.

As for other formats, my idea would be to convert them directly kinda? Idk though, makes more sense to just, convert it to an image and then to another format?
And there'll be 255 shades? Well, maybe. So as to be compatible with other color formats I suppose?

EX;
And just for an example that the user would see in the default workspace prior to adding any images, we'd have this string of characters;
nnnnnnnnnn
nwnwwwwnwn
nnnwwwwnnn
nwnwwwwnwn
nnnnnnnnnn
^ which is just a simple little illustration for the viewer, to see what our program does


Other things;
We'll have the image rescale to fit within a 10/29.5 height and 10/52.5 width ratio, assuming that 29.5cm and 52.5cm are the dimensions of your screen(excluding the plastic borders of your screen that don't emmit light), with the 10 being 10cm, but both fractions representing the amount of space on your screen that the preview image for the image-result & image-import we put in via the import button just under the preview image-display.

Images will retain all their pixels!
We will also be storing the modifiers in a seperate image layer, which will be made so as to be able to recreate the image in its entirety.

We will have a multi-choice for the modifier colors to be enabled/disabled/displayed seperately.
Edit: Same will be true for the third layer, the "Cleanup-channel"

EXTRA Clarification on what the layers are;
ROYGCBIVPM+NWbg = the "simplified-channel".
The modifer layer = the "shading-channel"
And for the third layer, well the cleaner-layer = the "Cleanup-channel"


Default settings;
The other 2 channels, will be disabled by default.
The example text-mapping of the so-called video-icon(not a class of image, that's just what its called), will be displayed by default, but will be gone immediately after the user imports an image or deletes the text that its converting from.
