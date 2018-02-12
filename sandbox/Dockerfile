FROM clojure:lein-2.8.1

RUN curl -sL https://deb.nodesource.com/setup_8.x | bash - \
  && apt-get update \
  && apt-get install -y maven nodejs php7.0 \
  && apt-get --purge autoremove -y \
  && curl -sS https://getcomposer.org/installer | php \
  && mv composer.phar /usr/local/bin/composer \
  && npm install -g lumo-cljs --unsafe-perm

ENTRYPOINT ["bash"]
