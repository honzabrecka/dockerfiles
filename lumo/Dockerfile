FROM clojure:boot-2.7.2

RUN curl -sL https://deb.nodesource.com/setup_8.x | bash - \
  && apt-get install -y nodejs \
  && apt-get --purge autoremove -y \
  && npm install -g lumo-cljs --unsafe-perm

CMD ["/usr/bin/lumo"]
