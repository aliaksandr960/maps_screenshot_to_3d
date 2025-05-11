# Converting Google Maps Screenshot to 3D Model in a Single Jupyter Notebook

### Recently, several high-quality monocular depth estimation models have been released, such as Apple's DepthPro. Inspired by this, I created a simple playground to experiment with generating point clouds and 3D models from aerial imagery—specifically Google Maps screenshots.

### Pipeline Overview:
1. Load the image
2. Estimate depth and invert it to represent height instead of distance from the camera
3. Remove background using MinPool subtraction
4. "Unscrew" the perspective by applying horizontal and vertical shifts
5. Visualize the resulting mesh or point cloud


*Plotly (Web): Enables in-notebook mesh viewing, but rendering is sometimes buggy—you may need to click buttons more than once to refresh.*
*Open3D (GUI): Produces smooth and high-quality point clouds, but only runs locally. On Linux systems, you may need to configure environment variables.*

 ### Licensing:
 - The notebook code is released under the MIT License.
 - Model weights and dependencies are licensed by their respective authors.


