FROM golang:1.21-bullseye@sha256:ca78a56712ab89487123b3af2b30052824653730e7ff25271d2f3037153bc0df

RUN GO111MODULE=on go install sigs.k8s.io/controller-tools/cmd/controller-gen@v0.10.0
RUN GO111MODULE=on go install k8s.io/code-generator/cmd/conversion-gen@v0.25.4

RUN mkdir /gatekeeper
WORKDIR /gatekeeper
