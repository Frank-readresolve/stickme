# Katathon stickme
Un mélange de katas et de hackathon :)

## Présentation, objectif général
Vous devez réaliser, en binôme, une application de gestion et de mise en avant de stickers. Les fonctionnalités attendues sont décrites sous forme d'issues GitHub et associées à un board non trié, le tout disponible dans ce repository.

Cette application doit être implémenté avec la stack suivante : Vue 3 (options API), Bootstrap 5.2, Spring boot 2.7.7 (Java 11, Maven), PostgreSQL.

Il n'est pas interdit de travailler en dehors des heures de formation.

Le travail doit être organisé (avec l'aide du formateur) pour que chaque membre du binôme intervienne sur toutes les couches de l'application, et participe à chaque étape.

## Barème de points, classement et prix
### Barème de points
Chaque fonctionnalité réalisée entièrement, fonctionnelle de bout en bout, rapporte 8 points. Si une fonctionnalité n'est réalisée qu'en partie, il n'y a aucun point. Si tout y est mais que l'écran ne correspond pas au wireframe validé en amont, la fonctionnalité rapporte 7 points au lieu de 8 :)

Certaines fonctionnalités ont des points bonus (cf. description des issues). Il n'est pas obligatoire d'implémenter ces bonus... Mais s'ils le sont, ils doivent être entièrement fonctionnels pour rapporter les points correspondants.

Le katathon sera ponctué de 2 Kahoot! à l'issu desquels les équipes remporteront un nombre de points proportionnel au taux moyen de bonnes réponses (moyenne dans l'équipe car tous les membres participent). Par exemple, si un Kahoot! a 10 questions et que le binôme répond correctement à 60% (1 avec 40% et l'autre avec 80% par exemple) en moyenne alors ça rapporte 6 points à l'équipe.

Super bonus de 10 points si tout est entièrement implémenté, incluant les bonus.

### Jokers
Chaque binôme a le droit à 2 jokers par demi-journée, non cumulables, techniques ou fonctionnels. Chaque joker utilisé fait perdre 2 points.

### Classement et prix
Les 2 membres de l'équipe totalisant le plus grand nombre de points remportent chacun un exemplaire de "Chief Bullshit Officer" de Fix.

Tous les membres des équipes 2 et 3 sur le podium (au nombre de points) remportent un lot de stickers sur la stack du katathon.

Un classement intermédiaire sera publié en chaque fin de journée.

### Perturbations
Le formateur va procéder régulièrement à des revues de code et des tests UAT et faire des retours, avec plus ou moins de précisions, qu'il faudra obligatoirement traiter. Autrement formulé, si les corrections ne sont pas prises en compte, la ou les fonctionnalités concernées ne seront pas considérées comme terminées...

Bien s'organiser quand des corrections sont demandées. Discuter dans l'équipe, comprendre la revue de code, estimer grosso modo, assigner.

## Étapes à suivre
1. Créer un repository "private" nommé "katathon-stickme" sur le compte GitHub d'un des membres du binôme, ajouter l'autre membre et le formateur en collaborateurs
2. Prendre connaissance des issues, les reproduire dans un board du repository, mais uniquement avec le titre pour gagner du temps (description pas indispensable). Échanger et proposer un ordre dans lequel l'équipe souhaite implémenter les fonctionnalités, cet ordre doit apparaître dans le board
3. Identifier les tâches de la 1ère fonctionnalité. Ajouter des issues dans le même board (ou un autre) afin de pouvoir les assigner dans l'équipe
4. Faire valider les 3 premières étapes par le formateur avant d'aller plus loin. L'objectif principal est de partir avec une liste de taches bien identifées et bien réparties (ça ne compte pas comme joker...). Une fois la manière de travailler validée, à vous de jouer pour l'organisation de l'ensemble du katathon
5. Procéder au wireframing de chaque écran (sauf pour la fonctionnalité "delete sticker"), versions desktop et mobile, avant de commencer toute implémentation. Ces wireframes doivent être validés par le formateur. Chaque membre de l'équipe doit participer, il y a 5 fonctionnalités à wireframer, le partage peut être de 2 vs 3 chacun. Le binôme discute pour un rendu cohérent mais chacun doit produire des wireframes. Libre choix du ou des outils. L'important est de pouvoir se projeter en tant que futur utilisateur. Communiquer les wireframes au formateur (peut importe comment) pour vérifier que les écrans correspondent bien après implémentation et valider les points bonus ! Cependant il est possible de proposer de nouvelles versions de wireframes...
6. C'est parti mon kiki !

## Tips et contraintes
La contrainte la plus forte est de s'organiser pour que chacun fasse un peu de tout (contexte de formation). Vous pouvez, grosso modo, avoir trois organisations :
1. Spécialisée : chaque fonctionnalité est découpée en deux, la partie front et la partie back (API + DB), chaque membre s'occupe d'une des parties puis vous faites des rotations de fonctionnalité en fonctionnalité
2. Fullstack : chaque membre prend en charge une fonctionnalité et implémente le front et le back. Plus difficile au démarrage car il faut initialiser les projets et on risque plus de se marcher un peu sur les pieds et d'avoir des conflits
3. Mixte : spécialisée puis fullstack

Le pair programming mais avec rotation est une autre approche.

Penser à partager le code régulièrement sur GitHub.

Bien s'entendre sur les différentes conventions (formatage, nommage...)

### Contraintes techniques
1. Mono repository
2. Trois projets, un pour chaque couche, chacun sont .gitignore adapté
3. Les scripts DDL et DML doivent pouvoir être rejoués
4. Le script DDL définit toute le schéma, un seul script donc
5. Le script DML doit insérer au moins 10 stickers, dans les règles de l'art...
