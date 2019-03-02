# Deep Bounding Box Regression using Keras

A Keras model to infer bounding box coordinates of synthetic black images with white boxes

## Getting Started

- Clone the repo into your folder

    `git clone https://github.com/sanjeev309/deep_bbox_regression_keras.git`

- Launch `jupyter notebook` in the repo directory and open the notebook `keras_bbox_regression.ipynb`


## Prerequisites

Keras, Matplotlib, OpenCV 3.2

## Summary

Deep Models are good for tasks of classification. However they can also be utilised to solve regression problems.

Using Deep regression, a CNN model with Dense end nodes can be utilised to predict the 4 coordinates

of a bounding box namely (x1,y1) and (x2,y2)

For example:

Given the input image (100 * 100):

![](https://imgur.com/aY3zw9G.jpg)

The ideal model predicts the bounding box coordinates :

`[0.37, 0.31, 0.91, 0.81]`

which when rescaled to the image corresponds to 

`[37, 31, 91, 81]` 

        i.e. (x1,y1) = [37,31] {Top-Left Coordinate}
    
             (x2,y2) = [91,81] {Bottom-Right Coordinate}


## Author

* **Sanjeev Tripathi** - [LinkedIn](https://www.linkedin.com/in/sanjeev309/)


## License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/sanjeev309/deep_bbox_regression_keras/blob/master/LICENSE) file for details

## Acknowledgements

 - The database is generated by the tool available here : [synthetic_bbox_regression_db_tool](https://github.com/sanjeev309/synthetic_bbox_regression_db_tool)
 - The loss function has been used from a different repo that I cannot locate. This Ack will be updated soon.