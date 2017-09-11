FROM clojure:lein-2.7.1

RUN curl -sL https://deb.nodesource.com/setup_8.x | bash - \
  && apt-get install -y nodejs \
  && apt-get --purge autoremove -y

ENTRYPOINT ["bash"]
