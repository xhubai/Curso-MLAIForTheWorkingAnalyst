FROM miniconda

LABEL maintainer=@abel-losada

RUN conda update conda && \
  conda install --quiet --yes ipython && \
  conda clean -tipsy

CMD [ "ipython" ]