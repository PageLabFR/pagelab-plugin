# PageLab

PageLab est un service pour **cabinets d'avocats accompagnés** : il donne à votre assistant d'IA l'accès aux dossiers de votre cabinet pour dire où en est un dossier, quelles pièces manquent, quelles audiences approchent, quels honoraires sont impayés, et pour préparer des brouillons de relances, de courriers et d'actes avec leurs pièces sources. Il recherche aussi les textes de loi et les décisions de justice sur Légifrance et Judilibre, avec le lien officiel.

**PageLab n'envoie jamais rien** : il prépare des brouillons, l'avocat relit et envoie lui-même.

> Contenu préparé avec l'aide de l'IA : à vérifier par l'avocat avant tout usage. PageLab ne donne pas de conseil juridique et ne calcule aucun délai de procédure.

## Accès réservé

Le service est réservé aux cabinets accompagnés par PageLab : il n'y a pas d'inscription en ligne. Sans compte, l'installation de ce plugin mène à un écran de connexion qui explique comment **demander un accès** (écrire à contact@pagelab.fr).

## Installer

1. Dans Claude, ouvrez **Personnaliser > Plugins**, trouvez **PageLab** dans l'annuaire et ajoutez-le.
2. Ouvrez l'onglet **Connecteurs** du plugin et connectez PageLab : vous vous connectez avec les identifiants de votre cabinet, puis vous autorisez l'accès.

## Utiliser

Posez vos questions en français (« Qu'est-ce que j'ai aujourd'hui ? », « Où en est le dossier REC-2026-033 ? », « Quelles pièces manquent ? ») ou utilisez les commandes :
`/pagelab:ma-journee`, `/pagelab:ma-semaine`, `/pagelab:mes-audiences`, `/pagelab:mes-impayes`, `/pagelab:prepare-pour-moi`, `/pagelab:mon-courrier`, `/pagelab:point-dossier`, `/pagelab:pieces-manquantes`, `/pagelab:jurisprudence`, `/pagelab:verifier-mes-citations`, `/pagelab:conflits`, `/pagelab:mon-closing`, `/pagelab:noter-mon-temps`, `/pagelab:compte-rendu`.

Le plugin contient une courte consigne par agent (Sources, Pièces, Audiences, Honoraires, Sociétés, Nouveaux clients, Veille, Rédaction, Comptes rendus, Temps et facturation, Conformité) et une pour configurer le cabinet. Les agents activés pour votre cabinet sont réglables dans PageLab.

## Données et fonctionnement

- Le plugin ne lance **aucun programme** sur votre ordinateur : il contient seulement des fichiers texte (instructions et commandes) et l'adresse du serveur PageLab, `https://app.pagelab.fr/mcp`.
- Quand vous posez une question sur un dossier, Claude appelle le serveur PageLab, qui renvoie des réponses où les noms sont remplacés par des rôles (« Client REC-… ») lorsque votre cabinet a activé la pseudonymisation. Rien n'est stocké par le plugin lui-même.
- Les données de vos dossiers sont hébergées en France ; voir la [Privacy / politique de confidentialité](https://app.pagelab.fr/confidentialite) et la page [Sécurité](https://app.pagelab.fr/securite).
- Les méthodes détaillées, les modèles et les règles ne sont pas dans ce dossier : elles sont servies par le serveur, uniquement aux utilisateurs connectés.

## Marque et licence

« PageLab » est une marque. Ce plugin fonctionne avec Claude ; il n'est ni parrainé, ni approuvé par Anthropic. Dossier publié « tous droits réservés » (voir le fichier LICENSE).

## Support et sécurité

contact@pagelab.fr. Pour signaler une faille : voir https://app.pagelab.fr/securite.
