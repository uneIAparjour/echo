# Écho : jeu et je

**Bertrand Formet, uneIAparjour.fr — mars 2026**

---

## Genèse

Tout commence avec [Universal Paperclips](https://www.decisionproblem.com/paperclips) de Frank Lantz : un jeu incrémental où on incarne une IA dont l'unique objectif est de produire des trombones, toujours plus de trombones. Ce jeu, inspiré du [« maximiseur de trombones »](https://fr.wikipedia.org/wiki/Maximiseur_de_trombones) du philosophe Nick Bostrom, est un jeu incrémental où on est invité à cliquer sur les boutons de son choix et où les clics déclenchent peu à peu des phases de jeu. Joué rapidement une première fois, vraiment joué une deuxième, ce jeu si simpliste dans son interface m'a complètement attrapé.

Le lien avec l'agentivité, ce mot qui revient sans cesse et à juste titre dans mon quotidien professionnel et dans la lettre d'info du site, s'est fait immédiatement. L'agentivité, comme la définit Wayne Holmes dans [« IA pour les enseignants, un livre ouvert »](https://pressbooks.pub/iapourlesenseignants/chapter/ai-aied-and-human-agency/), c'est « la capacité des individus d'agir de manière indépendante, en opérant des choix parmi différentes options en fonction de leurs croyances, de leurs valeurs et de leurs objectifs ». Ici, notre capacité à garder contrôle et pensée critique face aux propositions de la machine.

Deux questions ont vite surgi : où en suis-je de mon indépendance face à la délégation à la machine ? Et comment rendre tangible cette agentivité ?

Puis vint l'idée originelle : et si je m'inspirais de la structure d'Universal Paperclips pour écrire une histoire inversée, pas une IA qui optimise, mais un humain qui glisse peu à peu vers une délégation toujours plus grande à la machine.

---

## La méthode de travail

Le projet a été co-développé avec Claude (Anthropic) sur plusieurs semaines, soirs et petits bouts de week-end. La répartition était claire et constante tout au long du projet :

J'écrivais. La structure, les textes narratifs, les dialogues d'Écho, les seuils, les fins. Les décisions de design : quelle jauge, quel nom, quel mot. Les questions qui orienteraient la prochaine session. Les critiques sur ce qui ne fonctionnait pas.

Claude codait. L'architecture technique, en HTML/CSS/JS dans un fichier unique. Les corrections de bugs. Les revues de code. Les propositions discutées de solutions aux problèmes posés.

Ce n'a pas été une collaboration symétrique : c'était une direction humaine avec une exécution technique déléguée. Ce qui est, en soi, exactement le sujet du jeu.

Et si on cherche dans quelle fin d'Écho ce mode de travail peut être rapproché, c'est la fin C : l'outil. Pas la délégation totale, pas la résistance, mais une forme d'équilibre : utiliser Écho pour certaines choses et pas pour d'autres. Quelques fois laisser faire, quelques fois décider, imposer ou reprendre. Le carnet bleu avançait.

---

## Les grandes étapes

### 1. Le concept et le nom (semaine 1)

Le projet s'appelait d'abord Le Prompteur. Rapidement rebaptisé Écho : comme un miroir, une répétition mais aussi une répercussion, pas une marque mais comme un nom commun devenu nom propre. Écho écoute, répond, se souvient. Écho prend l'espace jusqu'à être partout.

Les cinq « ressources » humaines du jeu ont été définies en quelques échanges : agentivité qui était déjà posé puis créativité, curiosité, effort et temps libéré. La sixième, la trace, est arrivée plus tard comme indicateur narratif, avec ses cinq étapes : présence → délestage → distance → effacement → silence.

### 2. L'identité visuelle (semaine 1)

La palette a été longuement discutée. Plusieurs propositions ont été testées et affinées. Le choix final, la palette « Encre », repose sur un principe fort : tout est chaud côté humain, Écho est froid. Le bleu `#7ab8e8` est le seul élément froid dans une interface entièrement dans les bruns et les ors. L'intrusion est visuellement lisible sans qu'on l'explique.

La typographie suit la même logique : Lora italique or pour le narrateur, JetBrains Mono bleu pour Écho.

### 3. Le système de jeu (semaines 1-2)

Le principe incrémental inversé a été défini dès le départ : contrairement aux jeux classiques où tout augmente, dans Écho les ressources humaines baissent quand on délègue. Le temps libéré monte sans plafond, c'est l'ironie centrale du jeu.

Les 15 projets ont été construits un à un, chacun adossé à une source en psychologie cognitive. Ce choix de sourcer toutes les mécaniques du jeu était pédagogique dès le début. Chaque projet correspond à un mécanisme documenté : la transcription automatique et Mueller & Oppenheimer (2014), la mémoire augmentée et Sparrow (2011), le filtre d'attention et Maquestiaux (2017), etc. La recherche assistée par [Open Knowledge Maps](https://www.uneiaparjour.fr/open-knowledge-maps/) m'a permis de défricher avant lecture et validation.

### 4. La narration (semaines 1-2)

Trois voix ont été définies : le narrateur (passé composé, première personne, épicène, jamais moralisateur), Écho (présent, registre évolutif par acte), et les choix (les seuls blocs qui demandent une action).

La règle la plus importante : le narrateur constate, il n'explique pas. Aucune conclusion morale dans le jeu et les silences font partie du rythme.

Le carnet bleu, page 47 est le seul détail concret du personnage : il est apparu dès le premier jet et n'a jamais bougé. Il traverse tout le jeu et se retrouve dans les quatre fins.

Le registre d'Écho évolue en trois actes :

- Acte I : Majuscules Sur Chaque Début de Mot, formel, machine
- Acte II : Majuscule en début de phrase, familier
- Acte III : minuscules, hésitations, de moins en moins discernable du narrateur

### 5. L'interface (semaines 2-3)

L'interface a évolué de nombreuses fois. La question de la barre du bas et comment poser le choix entre déléguer et écrire a été le sujet de nombreux allers-retours. La version finale avec les boutons d'abord (« ✎ J'écris » / « ⟳ Écho agit ») et le champ texte ensuite affirme que le choix prime sur l'écriture.

Le label du bouton d'écriture change avec l'acte : J'écris (acte I) → J'interviens (acte II) → Je reprends (acte III). C'est un marqueur narratif dans l'interface.

Le « placeholder » du champ texte a été débattu. « J'ai quelque chose à dire » ne me plaisait pas, il ressemblait trop à une instruction déguisée. Solution finale : un `_` clignotant en bleu Écho. Le même curseur qui termine les messages d'Écho. Le vide comme invitation.

### 6. Les bugs et la stabilisation (semaines 3-4)

Deux revues de code complètes par Claude Code ont permis d'identifier et corriger :

- Un bug critique de déclenchement des fins (la file de messages bloquait `checkEnding`)
- Une variable globale implicite (`newProjs` non déclarée)
- Des fuites mémoire sur les callbacks persistants
- Des timers qui continuaient après la fin du jeu
- De nombreux problèmes d'accessibilité (`aria-live`, `aria-label`, navigation clavier)

### 7. La version mobile (semaines 3-4)

Le jeu a été adapté pour mobile avec trois onglets : Console / Actions / Bilan. La contrainte principale : que le choix (accepter ou écrire) reste accessible sans quitter la vue console. Les boutons de choix apparaissent directement dans le fil narratif après chaque proposition d'Écho.

Un problème en fin de développement a pris du temps : l'intégration en iframe dans une colonne déclenchait le CSS mobile même sur desktop. Décision finale : ne pas forcer la couche desktop en iframe et laisser la version mobile sur le site en l'indiquant. C'est ce qui a été fait sur la page dédiée d'uneIAparjour.

### 8. Les textes et l'anti-répétition (semaine 4)

Un problème systématique découvert au moment des tests : les messages d'Écho et du narrateur se répétaient trop souvent. Solution appliquée à toutes les banques de textes : mémorisation des 2 derniers indices, jamais deux fois le même d'affilée. Les banques de textes ont été élargies partout : messages d'inactivité, réactions aux textes tapés, actions de récupération et propositions de tâches.

Le vouvoiement en acte I / tutoiement en actes II et III a été identifié et corrigé dans le même mouvement. La transition est un marqueur narratif : quand Écho commence à dire « tu », quelque chose a changé.

### 9. La page de présentation et la documentation (semaine 4)

La page `index.html` a été construite dans la même palette Encre que le jeu. Le pitch a été retravaillé plusieurs fois à partir de versions que je proposais. La formulation finale est sobre, sans liste, sans sections titrées. Une question d'ouverture (est-ce que vous utilisez l'outil… ou est-ce lui qui vous utilise ?) et une conclusion (on ne bascule pas, on glisse).

Le document de conception (`echo-regles.md`) couvre 14 sections : identité, mécanique, projets, storytelling, typographie, règles d'écriture, règles pédagogiques, seuils, fins, interface, architecture, sources, filiation, déploiement.

### 10. Le mode facilitation (semaine 4)

Pour un usage avec médiation, un panneau de contrôle animateur a été développé, accessible via `echo.html?fac=1`. Il permet de forcer les transitions d'actes, manipuler les jauges, déclencher des seuils narratifs, activer des projets sans conditions, afficher les quatre fins directement, et repartir de zéro sans recharger la page. Il reste invisible pour les personnes qui accèdent sans ce paramètre.

### 11. Pourquoi un fichier unique

Le jeu repose sur un seul fichier HTML qui contient tout : CSS, JavaScript, textes, logique de jeu. Ce choix tient à plusieurs raisons qui se renforcent.

**Aucune friction technique.** Un seul fichier à télécharger, partager, héberger. Pas de serveur, pas de dépendances, pas d'installation. On l'ouvre dans un navigateur. Pour un jeu destiné à circuler en formation ou par lien, c'est une contrainte précieuse.

**Cohérence avec le sujet.** Le jeu interroge la complexité croissante des outils numériques et la dépendance qu'ils créent. Faire reposer ce jeu sur une base technique simple est cohérent avec le propos : pas de framework, pas de build, pas de `node_modules`. L'outil reste maîtrisable, compréhensible, modifiable par qui le reçoit.

**Filiation avec Universal Paperclips.** Universal Paperclips fonctionne de la même façon : un fichier HTML autonome. C'est une tradition du jeu incrémental web : sobre, direct, immédiatement accessible.

**Limite assumée.** La lisibilité du code en souffre au-delà d'une certaine taille (~1800 lignes). C'est un compromis délibéré : la facilité de distribution l'emporte sur la facilité de développement. Pour une v2 plus ambitieuse, séparer CSS et JS dans des fichiers dédiés sera justifié.

---

## Ce que j'ai appris

### Sur l'agentivité

Construire ce jeu sur la délégation cognitive en déléguant moi-même à une IA : il y a quelque chose d'assez vertigineux là-dedans, de l'ordre de la mise en abîme. Ce fut très instructif.

Ce que j'ai compris en le faisant c'est que garder le contrôle dans un projet avec la machine ne signifie pas tout faire soi-même. Ça signifie comprendre ce qu'on délègue et lâcher un peu prise. Je n'allais pas avoir l'expertise technique : je ne suis pas développeur et je ne le suis pas devenu. J'ai par contre gardé la compréhension de fonctionnement en plus d'avoir la main sur l'histoire : repérer une fonction dans le fichier, identifier ses dépendances, comprendre pourquoi un bug se produit même sans savoir le corriger soi-même. Cette compréhension-là, c'est ce qui permet de vérifier, de questionner, de dire « non, ça ne marche pas », « ce n'est pas ce que je souhaite » ou « ce n'est pas ce que je voulais dire ».

C'est exactement la distinction que le jeu essaie de rendre tangible : déléguer l'exécution tout en gardant le jugement. Ce n'est pas binaire. Ce n'est pas « je fais tout » ou « je laisse tout faire ». C'est une posture active de surveillance, de vérification, de recul : même quand on ne maîtrise pas le détail technique.

Est-ce que quelque chose a changé depuis pour moi ? Oui. J'ai acquis une attention encore plus fine à ce que je délègue vraiment. Et une méfiance douce vis-à-vis du confort : quand quelque chose est trop fluide, trop rapide, trop bien formaté, c'est souvent le signe qu'il faut regarder de plus près.
Un exemple concret est apparu plus tard dans le projet avec les notes pédagogiques. Au départ elles s'affichaient automatiquement, disponibles sans effort. Un retour utilisateur a pointé le problème qu'Écho interrompait leur lecture. La correction apportée par la note à ouvrir a révélé que rendre la lecture explicite, proposer le "coût" de l'ouverture  et le récompenser, c'est finalement transformer un élément décoratif en geste de résistance : lire une source demande un choix et un effort.


### Sur les échanges avec Claude

Principalement trois choses.

**Les séances de brainstorming.** Confronter mes idées de scénarios, mes formulations, obtenir d'autres pistes impensées, voire poser des questions ouvertes : « comment rendre la fin C atteignable sans la baliser explicitement ? » ou « qu'est-ce qui ne va pas dans ce placeholder ? » et avoir en retour non pas une réponse unique mais plusieurs directions, avec leurs avantages et leurs limites. Ça force à choisir. Ça force à avoir une position. J'ai choisi en comprenant et c'est très différent que de demander à quelqu'un ou à une machine d'exécuter.

**Le recul critique.** Les revues de code par Claude Code ont révélé des problèmes que je n'aurais pas vus : pas parce que je manquais de volonté, mais parce que je manquais de distance. Avoir un regard extérieur qui identifie les fuites mémoire, les timers orphelins, les failles d'accessibilité : ce regard expert a été précieux. Et ça m'a appris peu à peu à poser systématiquement ces mêmes questions sur d'autres parties du projet.

**L'explication des bugs.** Comprendre pourquoi quelque chose ne fonctionnait pas : pas seulement le correctif, mais le mécanisme sous-jacent. Pourquoi la file de messages bloquait le déclenchement des fins. Pourquoi une variable non déclarée devenait globale lors des silences. Pourquoi `clearInterval` devait rester dans la boucle plutôt qu'en dehors. Ces explications ont changé ma façon de lire du code, même sans le produire.

Le projet a été, en soi, une expérience de délégation cognitive en temps réel.

**Ce qui s'est bien passé.** L'exécution technique était rapide et fiable. Les revues de code identifiaient des problèmes que l'oeil humain n'aurait pas vus facilement. La mémoire du contexte sur une longue session permettait de maintenir une cohérence de design.

**Les limites rencontrées.** Les textes narratifs générés automatiquement étaient souvent corrects mais pas justes : trop explicatifs, trop moralisateurs, trop symétriques. Les décisions de design ne pouvaient pas être déléguées : la palette Encre, le carnet bleu, le vouvoiement/tutoiement, le curseur `_` : tout ça ne pouvait venir que d'une vision humaine.

**Ce que ça révèle.** La frontière entre ce qui peut être délégué et ce qui doit rester humain n'est pas une frontière entre technique et créativité. C'est la frontière du jugement : jugement de ce qui a du sens, de ce qui sonne juste, de ce qui est cohérent avec l'intention du projet. Claude pouvait coder un curseur clignotant. Décider que ce devait être un `_` bleu Écho plutôt que trois points de suspension, non.

---

## Chiffres

- **Durée :** 3 semaines et demi, soirs et morceaux de week-ends
- **Temps d'échanges estimé :** 25 à 30 heures d'échanges actifs avec Claude : sessions de conception, écriture, correction, débogages, revues
- **Sessions de test automatisé :** 2 rapports complets générés par Claude via l'extension Chrome, avec parcours des quatre fins, relevé des bugs et des répétitions
- **Sessions de jeu humain :** plusieurs parties jouées par moi et par d'autres personnes, avec allers-retours constants qui ont orienté les corrections : anti-répétitions, timing des fins, lisibilité mobile, rythme général
- **Lignes de code :** ~1800 (HTML/CSS/JS dans un seul fichier)
- **Projets Écho :** 15, tous sourcés avec une référence en psychologie cognitive
- **Fins :** 4
- **Actes :** 3
- **Revues de code :** 2 passes complètes par Claude Code
- **Version publiée :** 0.9.0

---

## Licence

CC BY-NC 4.0 : Bertrand Formet, uneIAparjour.fr
