ARG ELIXIR_VERSION=1.13.4
ARG OTP_VERSION=25.0.2
ARG DEBIAN_VERSION=bullseye-20210902-slim

ARG BUILDER_IMAGE="hexpm/elixir:${ELIXIR_VERSION}-erlang-${OTP_VERSION}-debian-${DEBIAN_VERSION}"

FROM ${BUILDER_IMAGE}
RUN apt-get update -y && apt-get install -y build-essential cargo git imagemagick cargo libjpeg62-turbo-dev libzbar-dev wkhtmltopdf
RUN apt-get clean && rm -f /var/lib/apt/lists/*_*