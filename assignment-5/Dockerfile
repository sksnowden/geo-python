FROM continuumio/miniconda3:24.7.1-0

WORKDIR /geo-python/assignment-5

# copy and install the conda environment
COPY environment.yml .
RUN conda env create -f environment2.yml

# log installed packages
RUN conda run -n a5-env pip freeze > installed_packages.txt

# set environment variables and shell
SHELL ["conda", "run", "-n", "a5-env", "/bin/bash", "-c"]
ENV PATH="/opt/conda/envs/a5-env/bin:$PATH"

# expose jupyterlab port
EXPOSE 8888

# start jupyter lab
CMD ["jupyter-lab", "--ip=0.0.0.0", "--no-browser", "--notebook-dir=/Users/sks49/geo-python/assignment-4"]
