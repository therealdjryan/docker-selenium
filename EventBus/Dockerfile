# !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
# NOTE: DO *NOT* EDIT THIS FILE.  IT IS GENERATED.
# PLEASE UPDATE Dockerfile.txt INSTEAD OF THIS FILE
# !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
FROM selenium/base:4.0.0-beta-3-20210802-djr
LABEL authors=SeleniumHQ

USER 222

#=================================
# Selenium Event Bus Configuration
#=================================

# Port where events are published
EXPOSE 4442
# Port where to subscribe for events
EXPOSE 4443
# Event Bus port
EXPOSE 5557

COPY start-selenium-grid-eventbus.sh \
    /opt/bin/

COPY selenium-grid-eventbus.conf /etc/supervisor/conf.d/
