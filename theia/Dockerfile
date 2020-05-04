FROM theiaide/theia-python:latest

ADD latest.package.json ./package.json
RUN yarn --cache-folder ./ycache && rm -rf ./ycache && \
    yarn theia build ; \
    yarn theia download:plugins

RUN pip3 install \
    python-language-server \
    flake8 \
    jupyter \
    azure-cli \
    autopep8 \
    matplotlib \
    bokeh

