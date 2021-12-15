# This is forked image based on the original project:
# https://github.com/osixia/docker-openldap 
# License: https://github.com/osixia/docker-openldap/blob/stable/LICENSE

FROM osixia/openldap:1.5.0
ARG BUILD_DATE
ARG VCS_REF
LABEL maintainer="Osixia <http://www.osixia.net>"
LABEL org.label-schema.build-date=$BUILD_DATE \
    org.label-schema.name="OpenLdap - Alpine" \
    org.label-schema.description="Provides a Docker image for OpenLdap DC on Alpine Linux." \
    org.label-schema.license=MIT(https://github.com/osixia/docker-openldap/blob/stable/LICENSE) \
    org.label-schema.vcs-ref=$VCS_REF \
    org.label-schema.vcs-url=https://github.com/osixia/docker-openldap \
    org.label-schema.schema-version="1.0"

ADD bootstrap /container/service/slapd/assets/config/bootstrap
ADD certs /container/service/slapd/assets/certs
ADD environment /container/environment/01-custom
