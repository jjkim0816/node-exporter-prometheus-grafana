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
    
- grafana 인 경우 dashboard template를 import 해서 사용하는게 좋다.
  import url : https://grafana.com/dashboards/22

