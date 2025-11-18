FROM jupyter/pyspark-notebook:latest

USER root

RUN pip install --no-cache-dir \
    pandas \
    matplotlib \
    seaborn \
    pyarrow \
    fastparquet

USER ${NB_UID}