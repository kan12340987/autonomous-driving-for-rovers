# autonomous-driving-for-rovers

This was a POC on introducing autodriving capabilities to a rover was developed as a final sem project. Autonomous path planning for rovers removes huge manual efforts required in manning a rover. This also results in significant time reduction. This POC was done by using technologies like Neural networks, image stitching and 3D reconstruction. 

The porject was divided into 5 phases:
1. **Image Stitching:** A panoromic 360* scene was created by stitching images together.
2. **Object Detection:** Object detection using YOLO was performed to detect rocks, boulders and pits. The panorama was annotated with the objects detected.
3. **3D Reconstruction:** These annotated images are reconstructed into 3D point clouds using 3D reconstruction. For 3D reconstruction, depth maps were generated to regain the depth information lost when a images are flattened on a 2D plane.
4. **Birds Eye View Generation:** The point clouds are flattened on 2D "Birds Eye" view map. This map will have the object detected during Object Detection as obstacles
5. **A-Star algorithm:** A-Star algorithm is performed on the "map" to find the path between two points.
