VX-S3DIS release (Fall 2024)

The **VX-S3DIS** dataset can be downloaded on [HuggingFace](https://huggingface.co/datasets/RemcoRoyen/VX-S3DIS).

The VX-S3DIS data is released in 2 zip-files. 'camera_view.zip' represents the dataset centered to the camera axis. 'global_view.zip' represents the global view of the scene where the points have their actual position in the 3D scene. The filename displays the underlying S3DIS room identifier.
The datasets consist of ply-files of the scenes. Important to note is that the order of the points reflect the order in which they were captured by the resolution scalable sensor, here the VoxelSensor Andromeda Simulator.

Each vertex contains the following information:

```
xyz - Vertex 3D position
rgb - Since the 3D sensor does not acquire color, these colors represent the semantic labels
label - The semantic label of the vertex
time - The time instance on which the vertex was captured
```

For additional information, we refer to the [RESSCAL3D++](https://arxiv.org/abs/2410.02323) paper.

Last updated: 2024-10-14
