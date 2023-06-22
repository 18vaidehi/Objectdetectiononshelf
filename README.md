# Shelf Image Annotation Visualization

This repository contains code for visualizing annotations on shelf images using Python. The code utilizes the `numpy`, `pandas`, `matplotlib`, and `imutils` libraries.

## Prerequisites

Before running the code, make sure you have the following dependencies installed:

- numpy
- pandas
- matplotlib
- imutils

You can install these dependencies using `pip` by running the following command:

```
pip install numpy pandas matplotlib imutils
```

## Getting Started

1. Clone the repository to your local machine or download the code as a ZIP file.

2. Open the code in your preferred Python development environment.

3. Update the file paths and URLs in the code according to your requirements. Specifically, make sure to update the following:

   - `train_images` variable: Specify the path to the directory containing the training images.
   - `master_df` variable: Update the URL or file path to the annotations.csv file.
   - `vis_annotations` function: If needed, modify the parameters of the function to customize the visualization.

4. Run the code. It will read the annotations from the CSV file and visualize them on the corresponding images.

## Additional Information

- The `train_images` variable is initialized with a list of image paths obtained using the `paths.list_images` function from the `imutils` library. This assumes that you have a folder named "train" containing the training images.

- The `master_df` variable reads the annotations from the provided CSV file using the `pd.read_csv` function from the `pandas` library. Make sure the file path or URL is correctly specified.

- The `vis_annotations` function takes an image path and a list of coordinate values as inputs. It visualizes the bounding box annotations on the image using matplotlib.

- The code includes a loop that iterates over the images in the "train" folder and calls the `vis_annotations` function to visualize the annotations for each image.

- Feel free to customize the code according to your specific needs.

## License

This project is licensed under the [MIT License](LICENSE).

## Sources

Link to dataset used: [gulvarol/grocerydataset](https://github.com/gulvarol/grocerydataset). Special thanks to the original authors for providing the dataset and annotation format.

Replaced GroceryDataset_part1/ShelfImages with this data https://storage.googleapis.com/open_source_datasets/ShelfImages.tar.gz

If you have any questions or issues, please feel free to open an issue in this repository.

Happy coding!
