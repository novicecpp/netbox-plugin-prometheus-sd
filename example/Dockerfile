FROM netboxcommunity/netbox:v4.2

RUN apt -y update && apt -y install git python3.12-venv

COPY ./plugin_requirements.txt /
RUN /opt/netbox/venv/bin/python -m ensurepip  \
    && /pip/opt/netbox/venv/bin/pip3 install  --no-warn-script-location -r /plugin_requirements.txt
