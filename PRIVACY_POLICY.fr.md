# Politique de confidentialité — Phone Monitor – Device Health

**Date d'entrée en vigueur :** 17 novembre 2026 · [English version](PRIVACY_POLICY.md)

Cette politique explique ce que fait l'application Android **Phone Monitor –
Device Health** (paquet `com.yan.phonemonitor`, « l'application ») des
informations présentes sur votre téléphone. Elle est publiée par mezyan
(« nous »).

## En bref

- Tout ce que l'application enregistre **reste sur votre téléphone**.
- L'application **n'a pas accès à Internet** : elle ne demande pas
  l'autorisation Android `INTERNET` et ne peut donc rien envoyer nulle part.
- Il n'y a **ni compte, ni publicité, ni statistiques d'utilisation, ni
  rapport de plantage**, ni bibliothèque de suivi tierce.
- Nous **ne voyons, ne collectons, ne vendons et ne partageons jamais** vos
  données.
- La sauvegarde dans le cloud d'Android et le transfert vers un autre
  appareil sont **désactivés** pour l'application : ses données ne sont pas
  copiées sur Google Drive ni sur un autre téléphone.

## Ce que l'application lit, et pourquoi

L'application est un outil de santé du téléphone. Pour fonctionner, elle lit
des informations sur votre téléphone auprès d'Android et enregistre les
résultats dans une base de données locale, sur le téléphone.

| Quoi | Pourquoi | Autorisation ou accès Android |
|---|---|---|
| Niveau de batterie, état de charge, température, tension, courant | Historique et santé de la batterie, alertes de température, planificateur « Tenir jusqu'à » | Aucune |
| Stockage libre et utilisé, taille de chaque application (appli, données, cache) | Historique du stockage, « Libérer de l'espace », applis les plus grosses et qui grossissent le plus | `PACKAGE_USAGE_STATS` (accès aux données d'utilisation) |
| Applications au premier plan et durée, écran allumé/éteint, déverrouillages | Temps d'écran, batterie par appli, limites quotidiennes, récapitulatifs | `PACKAGE_USAGE_STATS` (accès que vous activez vous-même) |
| Données Wi-Fi et mobiles utilisées par appli | Consommation de données, limites de données, forfait mobile | `PACKAGE_USAGE_STATS`, et uniquement sur Android 9 et versions antérieures `READ_PHONE_STATE` (exigé par les statistiques de données d'Android ; l'application ne lit ni votre numéro, ni vos appels, ni les identifiants de l'appareil) |
| Liste des applications installées, leurs noms, icônes et autorisations | Liste des applis, examen des autorisations (« Autorisations », « Surveillance de la confidentialité ») | `QUERY_ALL_PACKAGES` |

L'application n'utilise ni service d'accessibilité ni accès aux
notifications, et ne peut lire ni votre écran ni vos notifications.

L'application utilise aussi ces autorisations, qui ne donnent accès à aucune
donnée personnelle : notifications (`POST_NOTIFICATIONS`, pour les alertes et
les récapitulatifs), service au premier plan, maintien en éveil et démarrage
au lancement du téléphone (pour les relevés en arrière-plan et le moniteur en
direct), vibration et état du réseau. L'application ne demande pas à être
exemptée de l'optimisation de la batterie ; vous pouvez le faire vous-même
dans les paramètres d'Android si les relevés sont retardés.

## Où sont stockées les données

Tous les relevés, réglages et résultats sont stockés uniquement dans
l'espace privé de l'application sur votre téléphone. Les autres applications
ne peuvent pas les lire. Rien n'est envoyé, ni à nous ni à personne, car
l'application ne peut pas se connecter à Internet.

## Partage

Nous ne partageons de données avec personne. La seule façon pour des données
de quitter l'application est que **vous** choisissiez **Exporter** dans
Paramètres → Données et sauvegarde : l'application crée un fichier JSON et
ouvre le menu de partage d'Android, et c'est vous qui décidez où il va (par
exemple un fichier, un e-mail ou un stockage en ligne de votre choix). Le
fichier est ensuite traité par l'application ou le service que vous avez
choisi, selon sa propre politique de confidentialité.

## Durée de conservation et suppression

- Vous choisissez combien de temps l'historique est conservé dans
  Paramètres → Données et sauvegarde → *Conserver l'historique* (7, 30, 90,
  180 ou 365 jours, ou pour toujours ; 90 jours par défaut). Les relevés plus
  anciens sont supprimés automatiquement une fois par jour.
- **Supprimer tout l'historique** dans Paramètres → Données et sauvegarde
  efface tous les relevés. **Supprimer l'historique** sur la page d'une
  application efface les relevés de cette application.
- Désinstaller l'application, ou effacer son stockage dans les paramètres
  d'Android, supprime tout.

## Sécurité

Les données ne quittent jamais le téléphone et restent dans l'espace privé de
l'application, protégé par le cloisonnement des applications d'Android. Si
vous exportez un fichier, gardez-le dans un endroit sûr : il contient votre
historique.

## Enfants

L'application ne s'adresse pas aux enfants de moins de 13 ans et ne collecte
sciemment aucune information auprès de qui que ce soit, enfants compris.

## Modifications de cette politique

Si cette politique change, la nouvelle version sera publiée à cette adresse
avec une nouvelle date d'entrée en vigueur. Si une future version de
l'application devait un jour envoyer des données hors du téléphone, cela
serait indiqué ici et dans la fiche Google Play avant sa publication.

## Contact

Questions sur cette politique : [mezyantbe@gmail.com](mailto:mezyantbe@gmail.com)
