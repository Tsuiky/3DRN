<h1 align="center"> <p> 3DRN</p></h1>

<h2 align="center"> A Radiometric Correction based Optical Modeling Approach to Removing Reflection Noise in TLS Point Clouds of Urban Scenes</h2>

<p align="center">
<a href="" target="_blank">Li Fang</a><sup>a,e</sup>, 
<a href="" target="_blank">Tianyu Li</a><sup>a</sup>,
<a href="" target="_blank">Yanghong Lin</a><sup>b,e,*</sup>, 
<a href="" target="_blank">Shudong Zhou</a><sup>a</sup>,
<a href="" target="_blank">Wei Yao</a><sup>c,d</sup>,
</p>

<p align="center">
<sup>a</sup> Quanzhou Institute of Equipment Manufacturing Haixi Institutes, Chinese Academy of Sciences&nbsp;&nbsp; <br>
<sup>b</sup> Fujian Institute of Research on the Structure of Matter, Chinese Academy of Sciences&nbsp;&nbsp; <br>
<sup>c</sup> School of Engineering and Design, Technical University of Munich&nbsp;&nbsp; <br>
<sup>d</sup> GeoBIM & GeoNexus Intelligence&nbsp;&nbsp; <br>
<sup>e</sup> University of Chinese Academy of Sciences&nbsp;&nbsp; <br>
<sup>*</sup>Corresponding author. &nbsp;&nbsp; 
</p>

 Point clouds are vital in computer vision tasks such as 3D reconstruction, autonomous driving, and
robotics. However, TLS-acquired point clouds often contain virtual points from reflective surfaces, causing disruptions. This study presents a reflection noise elimination algorithm for TLS point clouds. Our innovative reflection
plane detection algorithm, based on geometry-optical models and physical properties, identifies and categorizes reflection points per optical reflection theory. We’ve adapted the LSFH feature descriptor to retain reflection features,
mitigating interference from symmetrical architectural structures. By incorporating the Hausdorff feature distance,
the algorithm enhances resilience to ghosting and deformation, improving virtual point detection accuracy. Extensive
experiments on the 3DRN benchmark dataset, featuring diverse urban environments with virtual TLS reflection noise,
show our algorithm improves precision and recall rates for 3D points in reflective regions by 57.03% and 31.80%,
respectively. Our method achieves a 9.17% better outlier detection rate and 5.65% higher accuracy than leading methods.

## Pipeline
<img src="model/overview .jpg" alt="Method" style="zoom:50%;">

## 💡 Data Set (Release soon)
The first introduced 3DRN contains 12 point cloud models with more than 55 million 3D points, collected by a terrestrial laser scanner (RIEGL VZ-2000i). All point cloud models are captured from real urban scene containing highly reflective areas with significant reflection noise, half of which are from Sanlinkou Innovation Park and the other half from Quanzhou Equipment Center. Each point in the point cloud model provides its XYZ position information and ground truth of the virtual points annotated by the professional. Figure shows a completed aerial view and partial scenes obtained after registration of all scan positions captured from the Sanlinkou Innovation Park, which clearly consists of real points and reflected virtual points.

<img src="model/detail.jpg" alt="Detail" style="zoom:50%;">
