ARG BASE_IMAGE=frappe/erpnext:v15

FROM ${BASE_IMAGE}

ARG FRAPPE_OIDC_EXTENDED_VERSION

USER frappe
WORKDIR /home/frappe/frappe-bench

RUN bench get-app \
    --branch ${FRAPPE_OIDC_EXTENDED_VERSION} \
    https://github.com/MohammedNoureldin/frappe-oidc-extended.git
