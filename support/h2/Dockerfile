# Open JDK 8 - Alpine
FROM java:openjdk-8-alpine

LABEL maintainer="mcerovski"

# File name of h2 zip
ENV H2_ZIP_NAME h2-2019-03-13.zip

# (from: http://www.h2database.com/html/main.html)
RUN wget http://www.h2database.com/$H2_ZIP_NAME && \
    unzip $H2_ZIP_NAME && \
    rm $H2_ZIP_NAME

ENTRYPOINT [ "/bin/sh", "/h2/bin/h2.sh" ]
