# Build the manager binary
FROM quay.io/operator-framework/helm-operator:v1.1.0

LABEL name="MVC-DB-App Operator" \
      vendor="ExampleCo" \
      version="v0.0.1" \
      release="1" \
      summary="This is an example of a helm operator for MVC-DB Application." \
      description="This operator will deploy MVC-DB-App to the cluster."
COPY licenses /licenses

ENV HOME=/opt/helm
COPY watches.yaml ${HOME}/watches.yaml
COPY helm-charts  ${HOME}/helm-charts
WORKDIR ${HOME}
