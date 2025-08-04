FROM mcr.microsoft.com/devcontainers/anaconda

RUN conda install -n base -c conda-forge mamba -y

RUN umask 0002 && \
  /opt/conda/bin/mamba env create \
  -n g420 \
  -c conda-forge \
  -y \
  python=3.11 jupyter ipykernel ipywidgets \
  geopandas mapclassify contextily affine \
  libgdal beautifulsoup4 descartes \
  fiona pyogrio folium networkx osmnx \
  numba rtree scipy scikit-learn seaborn pysal
