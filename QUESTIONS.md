# Information we have
4 classes:
- ["squiggle", "narrowband", "noise", "narrowbanddrd"]

Data is:
- training: 3200
- test: 800
- dimensions: (64, 128)


## Data Augmentation
Example of image augmentation
```python
datagen = ImageDataGenerator(
    zca_whitening = False,
    rotation_range = 0,
    zoom_range = 0.1,
    width_shift_range = 0.1,
    height_shift_range = 0.1,
    horizontal_flip = True,
    vertical_flip = False
)

datagen.fit(X_train)
```

# Architecture
- "A common mistake is to use convolutions with kernel too large"
    - an exception is for the first convolutional layer, like 5x5

### Good architectures to look at
- ResNet
    Important for training very deep architectures, uses skip connection for vanishing gradient problems to not end up with dead neurons
    $$
    f(x) = h(x)-x
    $$
- SENet (page 510) *Squeeze and Excitation Network*
    Extends inception and residual architectures, boosting performance by including a SEBlock

## Pooling Layers
- GlobalAvgPool2D: 
    A single output per feature map, extremely destructive, and only used before last layers
-

## output layer
Because they are classes: softmax
## Loss funciton
- "sparse_categorical_crossentropy"

___

## Tasks
- Separate data into training, validation, testing

- Hyperparameter Tunning's
    - training rate
- Modify Architecture
    - Implement dropout's
    - Compare them with different architectures
- After it work's, how it perform's with unseen data?

## Different Architectures by person
Changes on the Conv2D
- Fabi
    - 1st: (32,5,1)
    - 2nd: (64,3,1) 
- Ariana:
    - 1st: (64,5,1)
    - 2nd: (128,5,1)
- Nachicket:
    - 1st: (32,5,_)
    - 1st: (64,5,_)
- Fabian:
    - SENet; 
        - adding SE blocks (Squeeze and Exciation Network)
        - Add Residual unit's



# Question to Nina
- How many convolution layers to add
- Can transfer lerning if we use a different architecture?
- model.compile(loss="categorical_crossentropy", optimizer=optimizer, metrics=["accuracy"])
    - I did use "sparse_categorical_crossentropy" and got error's at training


# Idea


