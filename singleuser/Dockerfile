ARG DOCKER_NOTEBOOK_IMAGE
FROM $DOCKER_NOTEBOOK_IMAGE
ARG JUPYTERHUB_VERSION
RUN . /opt/conda/etc/profile.d/conda.sh && \
	python3 -m pip install --no-cache jupyterhub==$JUPYTERHUB_VERSION && \
	python3 -m pip install --upgrade jupyterlab-git && \
	conda install -c conda-forge jupyterlab jupyter_conda && \
	jupyter labextension install jupyterlab_toastify jupyterlab_conda




