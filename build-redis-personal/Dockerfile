
# Baixar a versão desejada
FROM redis:3.2.9

# Criar um diretório para o redis.conf
RUN mkdir -p /etc/redis
# Copiar o redis.conf do Servidor para a imagem
COPY redis.conf /etc/redis

# Definir o volume.
VOLUME ["/data"]

# Definir o diretório de trabalho
WORKDIR /data

# Executar o redis com o novo arquivo de configuração
CMD ["redis-server", "/etc/redis/redis.conf"]

# Expose ports.
EXPOSE 6379
