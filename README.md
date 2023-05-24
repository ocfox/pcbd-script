# Point Cloud Boundary Detection

This script demonstrates the process of reading a point cloud from a file, estimating normals, computing boundary points, and visualizing the results using the Open3D library. It also saves the computed normals to a text file.

## Prerequisites

Make sure you have the following dependencies installed:

- Python (version 3.6 or later)
- Open3D (version 0.13.0 or later)
- NumPy (version 1.19.0 or later)

## Usage

1. Download or clone the repository containing this script.
2. Place the point cloud file `Enschede-dataset.txt` in the same directory as the script.
3. Open a terminal or command prompt and navigate to the directory containing the script.
4. Run the following command to execute the script: `./`
5. The script will perform the following steps:

- Read the point cloud data from the file `Enschede-dataset.txt`.
- Estimate normals for the point cloud.
- Write the point cloud with estimated normals to the file `output.ply`.
- Read the saved point cloud from `output.ply`.
- Compute the boundary points of the point cloud with a distance threshold of 0.02 and a minimum number of neighbors set to 30.
- Print the number of boundary points detected and the total number of points in the original point cloud.
- Visualize the original point cloud (`pcd`) and the boundary points (`boundarys`) using a 3D visualization window.
- Save the computed normals to the file `normals.txt`.

6. After running the script, you will find the output point cloud file `output.ply` and the file `normals.txt` containing the computed normals in the same directory.

## Notes

- Make sure the input point cloud file `Enschede-dataset.txt` is in the correct format and contains valid 3D point data.
- Adjust the visualization parameters (`zoom`, `front`, `lookat`, `up`) in the script to customize the 3D visualization window according to your needs.

## License

This script is released under the [MIT License](LICENSE).
