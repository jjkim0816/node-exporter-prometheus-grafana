# prometheus
# node-exporter
# grafana

## build
- $ docker-compose up -d

## detail
- 마운트할 config 생성 : ${PWD}/etc/prometheus/prometheus.yml
- 기동 후static_configs 변경 ${PWD}/etc/prometheus/prometheus.yml
  - 물리적 서버에 docker로 기동시에는 prometheus docker 에 node-docker docker host 추가 필요
  - $ docker exec -u root -it [container id] /bin/sh
    $ vi /etc/hosts

