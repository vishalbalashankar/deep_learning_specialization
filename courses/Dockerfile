FROM jupyter/datascience-notebook

EXPOSE 8888

RUN conda install --quiet --yes plotly pyvis networkx && \
    jupyter labextension install jupyterlab-plotly --no-build && \
    jupyter lab build -y && \
    jupyter lab clean -y