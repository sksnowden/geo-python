FROM continuumio/miniconda3:24.7.1-0

WORKDIR /geo-python/assignment-4

COPY environment.yml .
RUN conda env create -f environment.yml

SHELL ["conda", "run", "-n", "a4-env", "/bin/bash", "-c"]
ENV PATH="/opt/conda/envs/a4-env/bin:$PATH"

EXPOSE 8888

CMD ["jupyter-lab", "--ip=0.0.0.0", "--no-browser", "--notebook-dir=/Users/sks49/geo-python/assignment-4"]

