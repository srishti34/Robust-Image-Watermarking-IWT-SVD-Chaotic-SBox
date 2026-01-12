# Robust Image Watermarking using Chaotic S-Box and IWT–SVD

I implemented a robust and secure digital image watermarking system using **Chaotic S-Box encryption combined with IWT–SVD**, and compared its performance with **DWT–SVD** and **DCT–SVD** techniques. The system is evaluated on multiple test images using **PSNR, SSIM, NCC, MSE, and BER** metrics, including robustness analysis under common image processing attacks.

## Techniques Used
- Chaotic S-Box based watermark encryption  
- Integer Wavelet Transform (IWT) with Singular Value Decomposition (SVD)  
- Discrete Wavelet Transform (DWT) with SVD (for comparison)  
- Discrete Cosine Transform (DCT) with SVD (for comparison)

## Methodology
- The host image is decomposed using IWT.
- The watermark is encrypted using a chaotic S-Box to enhance security.
- Singular Value Decomposition is applied to embed the encrypted watermark in the transform domain.
- Inverse transformation reconstructs the watermarked image.
- Watermark extraction is performed using the corresponding inverse process.
- Robustness is tested under various image processing operations.

## Evaluation Metrics
- **PSNR (Peak Signal-to-Noise Ratio)** – visual quality of the watermarked image  
- **SSIM (Structural Similarity Index)** – perceptual similarity  
- **NCC (Normalized Cross-Correlation)** – accuracy of extracted watermark  
- **MSE (Mean Squared Error)** – embedding distortion  
- **BER (Bit Error Rate)** – robustness of watermark extraction  

## Dataset
- Experiments were conducted on **15 grayscale test images**.
- Representative sample images are included in this repository.

## Results
Experimental results demonstrate that the proposed **Chaotic S-Box + IWT–SVD** method achieves **high imperceptibility and strong robustness** compared to **DWT–SVD** and **DCT–SVD** techniques. The proposed approach consistently yields **higher PSNR and SSIM values**, **lower MSE and BER**, and **improved NCC**, indicating better visual quality and more reliable watermark extraction across different test images and attack scenarios.

### Visual Results (IWT–SVD)

The following figure shows the complete watermarking process using the proposed IWT–SVD and Chaotic S-Box method, including the original image, watermark, watermarked image, and the extracted watermark.

![IWT-SVD Result](https://github.com/srishti34/Robust-Image-Watermarking-IWT-SVD-Chaotic-SBox/blob/main/results/screenshots/sample1.png?raw=true)


## How to Run
- Open the notebook from the `notebooks` folder.
- Run all cells sequentially in **Google Colab** or **Jupyter Notebook**.
- Required libraries are listed in `requirements.txt`.
