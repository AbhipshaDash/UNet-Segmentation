# UNet Segmentation
## Benthic Habitat Segmentation Using Multispectral Satellite Imagery

This project develops a deep learning model for benthic habitat segmentation using 8-band WorldView-3 satellite imagery from Guam. The goal is to classify each pixel into one of seven habitat classes:

* Background
* Seagrass
* Coral
* Macroalgae
* Sand
* Land
* Ocean

The project addresses challenges such as class imbalance, variable image sizes, and spectral similarity between underwater habitat types.

## Method

* Patch-based training using 256×256 image patches
* 8-channel U-Net architecture
* Weighted Cross-Entropy + Dice Loss
* Balanced sampling of rare habitat classes
* Data augmentation using horizontal and vertical flips

## Dataset

The dataset consists of multispectral WorldView-3 GeoTIFF imagery and expert-annotated habitat masks from Guam.

## Results

The model was evaluated on unseen images from Agana Bay and Manell-Geus and achieved strong segmentation performance across multiple habitat classes.

Detailed quantitative results, visualizations, and error analysis are available in the project report.

## Repository Structure

```text
code/       Training and evaluation scripts
results/    Predictions, figures, and evaluation outputs
report/     Final project report
```

## Technologies

* Python
* PyTorch
* NumPy
* OpenCV
* Rasterio
* Matplotlib

