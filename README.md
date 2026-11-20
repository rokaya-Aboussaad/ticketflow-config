# TicketFlow Config Repository

Repository de configuration consommé par Spring Cloud Config Server avec le profil `native`.

- `application.yml` : paramètres communs non sensibles.
- `*-service.yml` : paramètres propres à chaque service.
- Ne jamais committer de mots de passe, tokens, clés API ou certificats privés.
- En local Docker, le dossier est monté en lecture seule dans Config Server (`/config`).

Pour vérifier une configuration via Config Server : `GET http://localhost:8888/{application}/{profile}`.
