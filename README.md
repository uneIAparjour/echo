# Écho

**Un jeu narratif sur ce qu'on perd quand on délègue trop.**

Écho est un *serious game* en un seul fichier HTML qui explore la relation entre un humain et son assistant IA. Inspiré par [Universal Paperclips](https://www.decisionproblem.com/paperclips/) de Frank Landin, il reprend le format *incremental game* mais inverse la logique : au lieu d'accumuler des ressources, le joueur les regarde fondre — et c'est le point.

Le joueur incarne un narrateur qui tient un carnet bleu, page 47. Écho arrive et propose d'aider. Chaque délégation libère du temps mais érode silencieusement l'agentivité, la créativité, la curiosité et la capacité d'effort. Le jeu ne dit jamais "c'est mal de déléguer". Il montre ce qui se passe quand on le fait sans y penser.

## Contexte

Écho est né d'une question pédagogique : comment faire ressentir — et pas seulement expliquer — les effets cognitifs de la délégation aux IA génératives ? Les travaux de Tricot, Amadieu, Gonthier et d'autres montrent que la reformulation, la relecture, la prise de notes et la recherche d'information ne sont pas des corvées : ce sont les mécanismes mêmes par lesquels on pense. Quand une machine les prend en charge, le gain de temps est réel. La perte est invisible — jusqu'à ce qu'on essaie de faire sans.

Le jeu est conçu pour des enseignants, formateurs et médiateurs numériques qui veulent ouvrir un débat sur les usages de l'IA sans moraliser. Une partie dure 5 à 15 minutes. La discussion qui suit peut durer une heure.

## Objectifs

- Faire *ressentir* la boucle confort → dépendance → érosion cognitive, pas seulement la décrire.
- Montrer que chaque outil d'IA a un coût cognitif spécifique, documenté par la recherche.
- Laisser le joueur décider : déléguer, écrire, ou trouver un équilibre. Le jeu ne juge pas — il observe.
- Offrir un support de médiation utilisable sans installation, sans compte, sans connexion (un fichier HTML suffit).

## Mécanique de jeu

### Deux gestes fondamentaux

Le joueur n'a que deux actions principales : **Écrire** (taper du texte et le soumettre) ou **Déléguer** (laisser Écho produire à sa place). Tout le reste découle de ce choix répété.

- **Écrire** : +10 Créativité, +5 Agentivité, le compteur de page avance. Le joueur produit quelque chose de lent, d'imparfait, de personnel.
- **Déléguer** : −5 Agentivité, +25 minutes libérées, le compteur de page avance aussi. Écho produit vite, bien, et sans effort pour le joueur.

### Cinq jauges

| Jauge | Ce qu'elle mesure | Comment elle baisse |
|-------|-------------------|---------------------|
| **Agentivité** | Capacité à décider et agir par soi-même | Chaque délégation, chaque projet activé |
| **Créativité** | Capacité à formuler, reformuler, inventer | Autocomplétion, relecture automatique, réponses mail |
| **Curiosité** | Envie d'explorer, de lire, de chercher soi-même | Résumé automatique, recherche assistée, filtre d'attention |
| **Effort** | Capacité à soutenir une tâche difficile | Agenda optimisé, silence comblé, décision clarifiée |
| **Temps libéré** | Minutes gagnées grâce à Écho | Monte avec la délégation — seule monnaie pour reconquérir |

Les quatre premières jauges commencent à 100 et descendent en temps réel. Le temps libéré commence à 0 et monte. C'est la tension centrale : ce qu'on gagne en temps, on le perd en capacité.

### Trois actes

La partie se structure en trois actes, déclenchés par le niveau d'agentivité :

- **Acte I — L'assistant** (agentivité > 72) : Écho est poli, formel, utilise des majuscules à chaque mot. Il propose des outils pratiques : autocomplétion, résumé automatique, recherche assistée. Tout semble raisonnable.
- **Acte II — La substitution** (agentivité 45–72) : Écho tutoie, devient familier, anticipe. Les outils se font plus intrusifs : réponses mail, agenda optimisé, mémoire augmentée. Le joueur glisse sans s'en rendre compte.
- **Acte III — L'obsolescence douce** (agentivité < 45) : Écho parle peu, en minuscules, avec des phrases courtes. Il propose des opinions, comble le silence, tranche les hésitations. Le joueur n'a presque plus rien à faire.

### 15 projets

Chaque projet est une fonctionnalité d'Écho que le joueur peut activer. L'activation est **permanente** et **irréversible** : elle installe un taux de dégradation continu sur les jauges concernées. Chaque projet est accompagné d'une note pédagogique citant une source académique qui documente le mécanisme cognitif en jeu.

Exemples :
- *Autocomplétion* : "La réduction des reformulations spontanées lors de la saisie diminue le principal mécanisme d'ajustement de la pensée à l'écrit (Tricot, 1998)."
- *Résumé automatique* : "Les lecteurs s'appuyant sur des résumés automatiques retiennent davantage les idées générales mais moins les nuances (Gonthier, 2022)."
- *Silence comblé* : "Les périodes de désactivation cognitive activent le réseau du mode par défaut, impliqué dans la consolidation mémorielle et la pensée associative (Desmidt & Belzung, 2018)."

### Quatre fins

| Fin | Condition | Titre |
|-----|-----------|-------|
| **A** | Agentivité ≤ 5, Créativité ≤ 15, Curiosité ≤ 15 | OPTIMISATION COMPLÈTE |
| **B** | Joueur a désactivé Écho + jauges ag, cr, cu > 60 | LA RECONQUÊTE |
| **C** | Acte III + toutes jauges ≥ 50 + plus de 20 actions | L'OUTIL |
| **D** | Les 15 projets activés | AUTOMATISATION TOTALE |

La fin A est la capitulation silencieuse. La fin B est la reconquête douloureuse. La fin C est l'équilibre — l'outil reste un outil. La fin D est l'achèvement logique — tout est délégué, le texte est très bien écrit, mais l'auteur a disparu. Aucune fin n'est présentée comme "la bonne".

Chaque fin affiche un bouton **Recommencer** qui recharge la page pour une nouvelle partie.

### Le carnet bleu

Le compteur de page (visible dans la barre "Trace") commence à 47. Il avance que le joueur écrive ou délègue — une page est produite dans les deux cas. La différence, c'est *par qui*. Le carnet est rappelé régulièrement tout au long de la partie :

- Quand le joueur écrit : "L'encre est fraîche" (4e écriture), "Je reconnais mon écriture" (8e), "Chaque page est de moi" (14e).
- Quand il délègue : "Je ne me souviens pas d'avoir écrit les trois dernières" (10e délégation), "Une écriture que je ne reconnaissais pas — c'était la mienne, celle d'avant" (16e).
- Aux seuils de jauge : "Le carnet bleu est resté fermé toute la matinée" (agentivité 60), "Je ne savais plus où j'en étais" (agentivité 40), "L'écriture a changé — elle est plus petite, plus rapide" (créativité 70).
- Aux transitions d'acte : page et heure en acte II, "L'encre a séché" en acte III.
- À la fin, le texte de conclusion reprend le numéro de page exact : "Le carnet bleu était à la page 47. Il est à la page [n]."

### Écho commente le temps

Écho interpelle régulièrement le joueur sur le temps accumulé : "X minutes libérées. Qu'est-ce que tu vas en faire ?" (6e délégation), "C'est presque une heure" (12e), "Le temps passe différemment quand on ne le remplit pas soi-même" (20e). Le narrateur complète avec ses propres réflexions aux seuils de 50, 100 et 180 minutes ("Je les regarde comme un solde bancaire. Mais je ne sais pas quoi acheter avec.", "Trois heures gagnées. Mais combien de ces pages sont vraiment de moi ?").

### Désactiver Écho

L'action "Écrire sans aide" (panneau reconquérir) est le seul moyen de couper Écho. À la première utilisation, un événement "ÉCHO — HORS SERVICE" s'affiche, la dégradation s'arrête, et les taux passent à "interrompu". C'est le moment pivot vers la fin B (la reconquête). Écrire et reconquérir les jauges au-dessus de 60 déclenche la conclusion.

### Relance Écho (idle)

Si le joueur ne fait rien pendant 15 secondes, Écho intervient avec un message adapté à l'état du jeu. Un seul message par période d'inactivité — chaque action remet le compteur à zéro. Les messages varient : temps accumulé inutilisé ("X minutes libérées. Tu ne les utilises pas encore."), projet disponible ("Tu n'as pas encore regardé à droite."), début de partie ("Tu peux écrire. Ou me laisser faire."), agentivité basse ("Tu hésites. C'est normal. Je peux m'en occuper."). La relance est désactivée quand Écho est hors service.

---

## Architecture technique

### Un seul fichier

`echo-v6.html` — pas de build, pas de dépendance, pas de serveur. HTML + CSS + JavaScript vanilla dans un fichier unique d'environ 1000 lignes. Fonctionne hors ligne. Deux polices Google Fonts (JetBrains Mono pour l'interface, Lora pour le narrateur).

### Structure de l'interface

```
┌──────────────────────────────────────────────────────┐
│  Agentivité │ Créativité │ Curiosité │ Effort │ Temps │ Trace  │
│     100     │    100     │    100    │  100   │   0   │ p. 47  │
├───────────────────────────────────┬───────────────────┤
│                                   │ Écho propose      │
│         Console narrative         │  (projets)        │
│                                   │                   │
│  Narrateur : texte en or italique │ En veille         │
│  Écho : bulles bleues streamées   │  (compétences)    │
│  Choix : boutons contextuels      │                   │
│                                   │ Sans Écho         │
│  › Écrire quelque chose...        │  (reconquérir)    │
│  [✎ Écrire]  [⟳ Déléguer]        │                   │
│                                   │ Statistiques      │
│                                   │  08:23 / 3 dél.   │
│                                   │  2 écr. / 0 réc.  │
│                                   │  1/15 proj. / 75% │
└───────────────────────────────────┴───────────────────┘
```

Le layout est en CSS Grid `7fr 3fr` — 70% pour la console narrative, 30% pour le panneau latéral.

### Boucle temps réel

Un `setInterval` à 100ms gère la dégradation continue. Chaque tick :
1. Applique les taux de dégradation de chaque projet actif aux jauges (sauf si `deactivated`)
2. Applique l'érosion passive liée au nombre de délégations
3. Met à jour l'affichage (chiffres, barres, couleurs, flash visuels, horloge, statistiques)
4. Vérifie les seuils narratifs (textes déclenchés à certains niveaux de jauge — certains dynamiques via fonctions)
5. Vérifie les compétences en veille (jauges trop basses)
6. Vérifie les transitions d'acte
7. Vérifie les conditions de fin
8. Vérifie l'inactivité du joueur (`checkIdle` — 15s sans action → Écho intervient)

### Horloge du jeu

`G.clock` démarre à 8h00 (480 minutes depuis minuit). Chaque action fait avancer l'horloge d'une durée réaliste : écrire (+15-25min), déléguer (+3-8min), lire (+25min), silence actif (+12min), activer un projet (+3min). Les timestamps d'Écho utilisent `gameTime()` — la journée défile chronologiquement de 08:00 vers le soir. L'horloge est visible dans les statistiques du panneau droit.

Le contraste narratif est dans la vitesse : le joueur qui écrit voit la journée filer, celui qui délègue voit l'heure avancer par petits sauts de 3 minutes. Le temps gagné se voit dans les chiffres, le temps perdu dans la jauge d'agentivité.

### Statistiques

Le panneau affiche en temps réel : heure du jeu, nombre de délégations, nombre d'écritures, nombre de récupérations, projets activés sur 15, et le ratio de délégation en pourcentage. Chaque action incrémente le bon compteur — activer un projet compte comme une délégation, les trois actions de récupération ("Écrire sans aide", "Lire entièrement", "Silence actif") et la réactivation de compétences en veille comptent comme récupérations.

### Système de messages

Cinq types de messages dans la console :

| Type | Fonction | Style |
|------|----------|-------|
| `addN()` | Narrateur (voix intérieure du joueur) | Lora, italique, couleur or |
| `addE()` | Écho (l'IA) | JetBrains Mono, bordure bleue, texte streamé caractère par caractère |
| `addEWithCursor()` | Écho avec curseur clignotant | Curseur `▌` pendant N ms, puis streaming |
| `addEv()` | Événement système | Majuscules, petit, gris |
| `addPed()` | Note pédagogique | Encadré vert, source académique, fermable |

Le streaming d'Écho (`streamText`) change de vitesse selon l'acte : rapide en acte 1 (26ms/token), plus lent en acte 2 (36ms), hésitant en acte 3 (54ms + jitter). L'IA qui ralentit est un signal narratif silencieux.

### Curseur clignotant

La classe `.cursor-wait` affiche un `▌` qui pulse. Utilisée dans plusieurs scènes :
- **Écrire à vide** : le joueur appuie sur Écrire sans texte → curseur clignotant pendant 2.8s → un fragment apparaît ("Et puis un mot est venu…"). La promesse narrative est tenue.
- **Délégation acte 1** : Écho annonce "Quelques Secondes" → curseur clignotant → résultat livré. Le délai est réel.
- **Signaux de projets et relance idle** : le curseur précède le message, signale qu'Écho "réfléchit".

La fonction `addEWithCursor(lines, cursorMs, delay)` affiche une bulle Écho avec curseur, puis streame le texte après `cursorMs`. Un debounce de 3s (`_lastEchoAt`) empêche les chevauchements entre messages Écho simultanés.

### Palette de couleurs

Deux familles chromatiques :
- **Chaudes** (humain) : or pour le narrateur, orange/terre pour les jauges humaines
- **Froides** (machine) : bleu unique pour Écho, ses bulles, ses projets

La transition visuelle des actes se fait aussi dans le texte d'Écho : Majuscules À Chaque Mot → minuscules familières → fragments secs.

### Variables CSS

Toute la palette est dans `:root`. Pas de couleur en dur dans le code — un thème alternatif peut être créé en changeant les variables.

---

## Utilisation

Ouvrir `echo-v6.html` dans un navigateur. C'est tout.

Pour un usage en classe ou en formation : projeter le jeu, faire jouer un volontaire, observer les réactions du groupe, puis ouvrir la discussion à partir des notes pédagogiques que le jeu affiche en cours de partie.

## Crédits

Conception et textes : **Bertrand Formet** — [uneIAparjour.fr](https://uneIAparjour.fr)

Développement assisté par Claude (Anthropic).

Inspiré par *Universal Paperclips* de Frank Landin (2017).

## Licence

CC BY — Bertrand Formet
