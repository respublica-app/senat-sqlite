# Base DOSLEG du Sénat sous format SQLite

![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/respublica-app/senat-sqlite/postgresql-to-sqlite.yml?style=for-the-badge&logo=github&label=Actions&link=https%3A%2F%2Fgithub.com%2Frespublica-app%2Fsenat-sqlite%2Factions%2Fworkflows%2Fpostgresql-to-sqlite.yml)


Le Sénat publie chaque jour un dump de ses bases de données internes, l'une d'elle est la **base de données DOSLEG**, qui contient l'intégralité des dossiers législatifs depuis octobre 1977.

Un des inconvénients de cette base est qu'elle n'est disponible que via un dump PostgreSQL 8.4, version obsolète depuis plusieurs années et dont l'import dans les nouvelles versions est relativement compliqué. Ce dépôt utilise donc Github Actions pour **convertir cet export en base de données SQLite**, qui sera réutilisée pour être réinjectée dans la base de données de res:publica.

---

La base de données DOSLEG est disponible sous [une licence](https://data.senat.fr/licence/) autorisant le repartage tant que les crédits sont conservés et qu'aucune ambiguïté n'existe sur le caractère non-officiel des redistributions. À ce titre il est nécessaire de préciser clairement que ***ce dépôt de conversion n'est ni géré par, ni approuvé par le Sénat***.

---

La base de données DOSLEG originale est disponible ici : https://data.senat.fr/dosleg/

Ce dépôt utilise le logiciel [postegresql-to-sqlite](https://github.com/caiiiycuk/postgresql-to-sqlite) de [caiiiycuk](https://github.com/caiiiycuk/)
