## Concepts
- Convolutional Layer's have many filters:
    - each filter's learn different features, profucing each one a feature map; increasing dimensionality
    - each map share's neuron weights
    ```python
    conv_layer = tf.keras.layers.Conv2D(filter=32, kernel_size=7)
    filter_map = conv_layer(input_images)
    ```

- padding on convolutions:
    - `padding="valid"`: (may ignore some inputs) output width will be:
    $$
    \lfloor \frac{i_h - f_h + s_h}{s_h} \rfloor
    $$
    - `padding="same"`: add's 0 padding to help the convolution reach edges
    $$
    \lceil \frac{i_h}{s_h}\rceil
    $$

- Pooling layer
    - Contains no weights, only reduced dimensionality

- Local response normalization layer:
    Ensures that previous layer's learn a variety of features

- 

## Inception modules
- why Convolutional layer with 1x1 kernel
    - captures no spatial patterns, but pattern's across channels
    - reduce dimensionality
