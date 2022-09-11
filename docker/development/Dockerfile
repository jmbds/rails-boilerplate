FROM ruby:3.0.3-alpine

# GENERAL ENVS #
ENV APP_PATH /project
ENV APP_BIN_PATH "$APP_PATH/bin"
ENV PATH "$PATH:APP_BIN_PATH"
ENV HOME "$APP_PATH/docker/development/home"

# RUBY ENVS #
ENV BUNDLE_PATH /bundle
ENV BUNDLE_BIN "${BUNDLE_PATH}/ruby/3.0.3/bin"
ENV PATH "${PATH}:${BUNDLE_BIN}"
ENV BUNDLE_JOBS 4
ENV RAILS_ENV development

# NODE ENVS #
ENV NODE_ENV development

WORKDIR $APP_PATH

COPY ./bin/install-system-dependencies $APP_BIN_PATH/install-system-dependencies
RUN $APP_BIN_PATH/install-system-dependencies

RUN mkdir $BUNDLE_PATH && chown jmbds:jmbds $BUNDLE_PATH

USER jmbds

ENTRYPOINT [ "docker/development/entrypoint" ]

EXPOSE 3000