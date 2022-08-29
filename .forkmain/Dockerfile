FROM registry.cn-hongkong.aliyuncs.com/h8rdev/devbox

COPY --chown=gitpod ./ ./

RUN make build

EXPOSE 9090

CMD ["sh", "-c", "./prometheus --config.file=documentation/examples/prometheus.yml"]
