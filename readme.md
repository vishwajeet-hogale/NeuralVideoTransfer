# Neural Style Transfer
Neural style transfer is an optimization technique used to take two images—a content image and a style reference image (such as an artwork by a famous painter)—and blend them together so the output image looks like the content image, but “painted” in the style of the style reference image.

## Define content and style representations 

Use the intermediate layers of the model to get the content and style representations of the image. Starting from the network's input layer, the first few layer activations represent low-level features like edges and textures. As you step through the network, the final few layers represent higher-level features—object parts like wheels or eyes.  These intermediate layers are necessary to define the representation of content and style from the images. For an input image, try to match the corresponding style and content target representations at these intermediate layers.

The model used to get the intermediate layer results is <b>VGG19</b>

## Neural Video Transfer 
Every frame of the video is extracted and the tensorflow hub's stylization module is used to 
convert each frame into a particular style based on the style rference image.


