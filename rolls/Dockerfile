ARG BUILD_FROM
FROM $BUILD_FROM

ENV LANG C.UTF-8

# Install requirements for add-on
RUN apk add --no-cache jq

# Copy data for add-on
COPY smart-home-hub-1.0.jar /
RUN chmod a+x /smart-home-hub-1.0.jar

CMD [ "java", "-Xmx512m" ,"-jar", "/smart-home-hub-1.0.jar" ]