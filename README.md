# gcloud-ace-flashcards
> [FR] - Des pseudo-flashcards pour préparer l'examen de certification Google Cloud : Associate Cloud Engineer.

### Qu'est-ce qu'un stockage d'objets ?

C'est un système de stockage qui traite les données en tant qu'objets, tels que, par exemple, des fichiers. Google Cloud dispose d'un service de stockage d'objets : Cloud Storage.

### Quelle commande déclenche un déploiement via Cloud Deployement Manager?

```sh
gcloud deployment-manager deployments create
```

### Quelle commande permet de fractionner le trafic entre plusieurs versions d'un service App Engine ?

```sh
gcloud app services set-traffic [ops]
```

  
### Combien de temps Stackdriver stocke-t-il les logs qu'il a accumulé ?

Stackdriver stocke les logs pendant 30 jours.

### Quels sont les 3 types de rôles ?

Les 3 types de rôles sont :
- Primitifs ;
- Prédéfinis ;
- Personnalisés.

### Vrai ou faux : Une machine virtuelle (VM) créée via la commande gcloud compute instances create --machine-type=n1-standard-4 tweets-scrapper-py disposera de 2 CPU.

**Faux.** Le paramètre `--machine-type=n1-standard-4` signifie que la machine disposera de 4 CPU.

### Contre quel type d'attaque le service Cloud Armor protège-t-il ?

Il protège votre application des attaques par déni de service distribuées (DDOS).

### Un ingénieur Cloud vous attribue le rôle de App Engine Deployer. Quelles opérations pouvez-vous effectuer ?

Vous avez désormais accès en lecture aux paramètres de l'application et la possibilité de déployer de nouvelles versions d'un service.

### Vrai ou faux : Le cycle de vie d'une fonction Cloud dépend de celui de chacune des fonctions déjà déployées ?

**Faux.** Chaque fonction cloud s'exécute, de manière isolée, dans son propre contexte d'exécution et son cycle de vie est indépendant des autres fonctions.

### Dans la hiérarchie du service de computing App Engine, quel est le composant au plus bas niveau ?

Il s'agit des **instances**. En effet, une application peut disposer de plusieurs **services**, qui eux peuvent contenir plusieurs **versions**, qui elles peuvent être exécutées sur plusieurs **machines virtuelles** (ou instances).

###  Quels sont les 2 types d'environnements d'exécution App Engine ?

Les 2 types d'environnements d'exécution sont :

- App Engine Standard (Python, Go, Node.JS, Java, PHP, Ruby) ;
- App Engine Flex (Conteneurs Docker).

### Qu'est-ce que BigQuery ?

BigQuery est un service **OLAP** (OnLine Analytical Processing) entièrement managé par Google, qui scale à l'échelle du pétaoctet, qui utilise des tables relationnelles pour organiser les données et qui permet d'utiliser le SQL pour les requêtes.

### Quels sont les 5 types de load balancers ?

Les 5 types de load balancers sont :
- HTTP(S) ;
- SSL Proxy ;
- TCP Proxy ;
- Internal TCP/UDP ;
- Network TCP/UDP.


### Vrai ou faux : Les fonctions Cloud constituent une solution idéale pour exécuter de longs traitements.

**Faux.** Par défaut, l'exécution d'une fonction Cloud expire après 1 minutes. Le délai d'expiration (timeout) peut être allongé à maximum 9 minutes. En général, une fonction Cloud permet d'effectuer de courts traitements en réponse à un événements produit sur GCP, par exemple :

> Convertir des fichiers au format .pdf dès qu'ils ont uploadé dans un bucket Cloud Storage.
