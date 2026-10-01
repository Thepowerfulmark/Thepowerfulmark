# Mark Ediev

DevOps engineer · Belgrade, Serbia · Remote, hybrid or on-site

![Kubernetes](https://img.shields.io/badge/Kubernetes-k3s-326CE5?logo=kubernetes&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?logo=helm&logoColor=white)
![Argo CD](https://img.shields.io/badge/Argo%20CD-GitOps-EF7B4D?logo=argo&logoColor=white)
![GitLab CI](https://img.shields.io/badge/GitLab%20CI-FC6D26?logo=gitlab&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?logo=ansible&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-Debian-A81D33?logo=debian&logoColor=white)

## Обо мне

DevOps-инженер: больше четырёх лет в инфраструктуре, из них два с половиной года в DevOps. Строю CI/CD на GitLab, автоматизирую Linux-серверы через Ansible и поставляю продукт заказчикам через собственный apt-репозиторий. Собрал с нуля кластер Kubernetes (k3s) и перевёл на него рабочий проект.

## Что сделал

- Перевёл проект с Docker Compose на собранный с нуля Kubernetes (k3s): Helm-чарт, деплой через Argo CD (GitOps), сеть закрыта NetworkPolicy и iptables. Любое изменение идёт коммитом в git и так же откатывается.
- Поднял self-hosted GitLab с нуля за 10 дней во время code freeze и перенёс на него платформу. Выстроил флоу builder → dev → stage → prod.
- Ввёл поставку заказчикам через apt: пакеты собираются в CI, обновление и откат делаются одной командой.
- Развернул с нуля stage-окружения на Debian 13 с Ansible baseline и довёл их до регулярных релизов.
- Разбираю production-инциденты на стыке кода и инфраструктуры, после каждого оставляю постмортем и runbook.

## Стек

- **Kubernetes:** k3s, Helm, Argo CD, kustomize, NetworkPolicy, Headlamp
- **CI/CD:** GitLab CI (include-шаблоны, свои раннеры, Container Registry), GitHub Actions, SAST (gosec, gitleaks, SonarQube)
- **Автоматизация:** Ansible, Bash, Python, Terraform (базовый уровень)
- **Контейнеры и поставка:** Docker, Compose, Podman, systemd, deb, apt, reprepro
- **Данные и очереди:** PostgreSQL, TimescaleDB, Redis, RabbitMQ
- **Сеть и безопасность:** nginx, TLS и внутренний CA, iptables, FreeIPA/LDAP, VPN
- **Наблюдаемость:** Prometheus, Grafana, Loki, Zabbix

## Репозитории

- [k3s-gitops-platform](https://github.com/Thepowerfulmark/k3s-gitops-platform) - шаблон одноузлового k3s: Helm-чарт с backend, frontend, PostgreSQL и RabbitMQ, Argo CD с автосинхронизацией, сеть по умолчанию закрыта, CI и runbook.
- [service-delivery](https://github.com/Thepowerfulmark/service-delivery) - шаблон поставки Go, Python и frontend: Compose для разработки, deb-пакеты и архив с systemd-юнитами, релиз по тегу.
- [cluster-stand](https://github.com/Thepowerfulmark/cluster-stand) - стенд на Kubernetes через kustomize: PostgreSQL, Redis, RabbitMQ, приложение и миграции.
- [AnyType](https://github.com/Thepowerfulmark/AnyType) - self-hosted сеть синхронизации Anytype с документацией по эксплуатации.

## Как работаю

Если сервис снаружи не отвечает, а процесс при этом запущен, сначала смотрю диск, сеть, юниты и окружение. К коду перехожу, когда инфраструктура это уже не объясняет. Много работаю вместе с backend-разработчиками на Python и Go и пишу документацию так, чтобы новый инженер разобрался без устных пояснений.

## In English

DevOps engineer with 4+ years in infrastructure, 2.5 of them in DevOps. GitLab CI/CD, Ansible, apt-based delivery, and a Kubernetes (k3s) cluster built from scratch with Helm and Argo CD. Based in Belgrade, open to remote work.

## Связь

Telegram: [@hidden_pool1](https://t.me/hidden_pool1)
