
# Neural Style Transfer

Neural Style Transfer (NST) is a fascinating technique that allows for the combination of the content of one image with the style of another, producing a unique and visually compelling result. This project is based on the research paper "A Neural Algorithm of Artistic Style" by Leon A. Gatys, Alexander S. Ecker, and Matthias Bethge. By leveraging neural representations, NST effectively separates and merges the content and style from different images using a neural algorithm.


## Approach
This project employs the VGG19 pre-trained convolutional neural network (CNN), introduced by K. Simonyan and A. Zisserman in their paper "Very Deep Convolutional Networks for Large-Scale Image Recognition." VGG19 is known for its depth and simplicity, making it highly suitable for tasks like neural style transfer.
Key Points:

Model: VGG19 pre-trained CNN

Layers: 16 convolutional layers, 3 fully connected layers, 5 max-pooling layers

Parameters: 15,304,768 parameters (weights and biases)

### Methodology:

Image Transformation: Both content and style images are transformed into tensors.

Feature Extraction: The VGG19 model extracts features from five distinct layers for style and one layer for content.

Loss Evaluation: The model evaluates the loss associated with style and content features.

Gradient Descent: An iterative process minimizes the loss by making incremental adjustments to the generated image, enhancing visual quality and fidelity.
## Deployment

To deploy this project run

```bash
  pip install -r requirements.txt
```


## Usage
User can add their content and style images by providing the URL of the images using the wget command:

```javascript
wget -q -O content.jpg "https://example.com/path/to/your/content_image.jpg"
wget -q -O style.jpg "https://example.com/path/to/your/style_image.jpg"

```
### View the Result:

The generated image will be saved and can be viewed to see the combined effect of the content and style images.


## Acknowledgements

 - [Neural Style Transfer Paper](https://arxiv.org/abs/1508.06576)
 

