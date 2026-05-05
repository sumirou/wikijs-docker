FROM elasticsearch:9.3.4

RUN if ./bin/elasticsearch-plugin list | grep -q analysis-kuromoji; then \
    ./bin/elasticsearch-plugin remove analysis-kuromoji; \
fi && \
    ./bin/elasticsearch-plugin install analysis-kuromoji
RUN if ./bin/elasticsearch-plugin list | grep -q analysis-icu; then \
    ./bin/elasticsearch-plugin remove analysis-icu; \
fi && \
    ./bin/elasticsearch-plugin install analysis-icu
