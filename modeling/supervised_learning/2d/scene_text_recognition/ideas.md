- data
  - augmentation
    - need some more augmentation?
      - rotation
      - aspect ratio variation
      - etc.
    - balance
      - regular and irregular
      - word distribution
    - filter or ignore bad example
  - input size
    - larger, better?
  - aspect ratio
    - keep or not(train and evaluation)
    - how the aspect ratio will affect the performance when evaluation
  - color
    - need or not
- model
  - irregular
    - implicit learning
      - rectification module
        - original image or upsampled image as input of rectification module
        - more precise rectification method
        - verify the upper bound of the rectification module
      - deformable conv(v1 and v2)
    - explicit learning
      - design a dedicated model to learn the rectification like scene text detection
  - backbone
    - dedicated designed one maybe better
  - feature map before classification
    - 1d
    - 2d
  - language model(implicit or explicit)
    - need or not
    - how the language model will affect the performance when evaluation
  - objective
    - predict the number of characters in the image
      - this problem is easy, which may help us to debug the scene text recognition system
    - predict which character is in the image
      - this problem is easy, which may help us to debug the scene text recognition system
  - sequence
    - rnn may be substituted by cnn or transformer
    - we may get inspiration from speech recognition
    - output variable length sequence
      - decoder(rnn)
      - set a maximum length
        - ctc
        - classification
---
- objective
  - state of art performance
  - fully convolutional neural network
  - no rectification module
  - interpretable
