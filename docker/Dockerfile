FROM jupyter/datascience-notebook:latest
USER jovyan
WORKDIR /home/jovyan/work/tmp
ADD ./requirements.txt /home/jovyan/work/tmp
RUN pip install -r requirements.txt
WORKDIR /home/jovyan/work
# ADD . /home/jovyan/work

# WORKDIR /work
# ADD . /work

# RUN pip install -r requirements.txt

# RUN pip install jupyter-contrib-nbextensions
# RUN pip install jupyter-nbextensions-configurator
RUN jupyter contrib nbextension install --user
RUN jupyter nbextensions_configurator enable --user

