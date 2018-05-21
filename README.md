# Outcrops, Gee Whiz!

3D digital outcrop models are cool. **Gee Whiz** is it fun to spin them around! But now let's do something interesting with them.

## Dependencies

- `numpy`
- `matplotlib`
- `sklearn`

To do shapefile line projection:

- [pyproj](https://github.com/jswhit/pyproj)

To use mesh data instead of point cloud:

- [PyMesh](https://github.com/qnzhou/PyMesh) (Fair warning: install requires building a lot of `C++` dependencies.)

## Organization

`data/`: Input data, and slice frames directory (the latter not uploaded).

`media`: Presentation slides, figures, movies, and simple `ffmpeg` movie generation script.

`notebooks/`: Jupyter notebooks. See `README` inside for more info.

`models/`: `pickle`d `sklearn.ensemble.AdaBoost` model for HSV $\rightarrow$ class prediction

`mesh_process.py`: Data loading + point cloud slicing + some convenience functions. Should add some things, rename, and have `PyMesh` functionality in a seperate module.

