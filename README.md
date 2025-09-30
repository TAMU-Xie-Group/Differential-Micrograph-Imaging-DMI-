# Differential-Micrograph-Imaging-DMI-

In this work, we introduce differential micrograph imaging (DMI), a technique developed to reveal subtle microstructural changes associated with strain localization in polished and etched metallic samples subjected to mechanical loading. The method first applies image registration to suppress rigid body motion and global deformation. A pixel-wise subtraction from the undeformed reference micrograph then isolates contrast variations arising from localized strain. DMI does not require speckle patterning and leverages information from every pixel in the micrograph. In contrast, digital image correlation (DIC) relies on surface patterning, and its spatial resolution is fundamentally limited by the subset and speckle size. While DMI is a semi-quantitative technique, where heat map intensity correlates with relative strain magnitude, it does not provide exact strain values or directions. Nonetheless, DMI can serve as a complementary technique to DIC by enabling high-resolution visualization of localized microstructural changes, particularly in regions with complex features and subtle deformation-induced microstructure changes. 

DMI uses pixel-wise intensity differences, so it is sensitive to any gray-level change, and not only those caused by in-plane strain. Small variations from out-of-plane relief or illumination drift (common in quasi-in situ tests) can therefore generate false positives. To mitigate this, we compute registration residuals as the absolute difference between the reference image and the registered (aligned) image. Residuals are then scaled and clipped using a robust global cutoff, chosen as a high percentile of residuals, determined by residuals from all analyzed images. This normalization suppresses illumination-induced fluctuations and prevents outliers from dominating the dynamic range, yielding more stable DMI maps.

**How to use the code**

1) Have the images you want to analyze saved in a folder. 
2) Create a new folder for the output images.
3) Update the code with the file paths.
4) Make sure you change the file read type to the same file type as your images
5) Run the code!

**If you use this code in your research, please cite our paper:**

