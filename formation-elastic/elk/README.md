# Stack Elastic (ELK) sur Docker

Exécutez la dernière version de la [stack Elastic][elk-stack] avec Docker et Docker Compose.

Basé sur les [images Docker officielles][elastic-docker] d'Elastic :

* [Elasticsearch](https://github.com/elastic/elasticsearch/tree/main/distribution/docker)
* [Logstash](https://github.com/elastic/logstash/tree/main/docker)
* [Kibana](https://github.com/elastic/kibana/tree/main/src/dev/build/tasks/os_packages/docker_generator)

Autres variantes de stack disponibles :

* [`tls`](https://github.com/deviantony/docker-elk/tree/tls) : Chiffrement TLS activé dans Elasticsearch, Kibana (opt-in) et Fleet

> [!IMPORTANT]
> Les fonctionnalités [Platinum][subscriptions] sont activées par défaut pour une période d'[essai][license-mngmt] de **30 jours**. Après cette période d'évaluation, vous conserverez l'accès à toutes les fonctionnalités gratuites incluses dans la licence Open Basic de manière transparente, sans intervention manuelle requise et sans perte de données. Consultez la section [Comment désactiver les fonctionnalités payantes](#comment-désactiver-les-fonctionnalités-payantes) pour désactiver ce comportement.

---

## Résumé

```sh
docker compose up setup
```

```sh
docker compose up
```

**Tout effacer**

```sh
docker compose down -v
```