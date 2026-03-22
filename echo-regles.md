# Écho — Règles de conception
Document de référence.
Fichier de jeu : `index.html` — https://uneiaparjour.github.io/echo/

---

## 1. Identité du projet

### 1.1 Concept central
Le joueur est un humain qui interagit avec un assistant IA nommé **Écho**. Au fil du jeu, il délègue progressivement ses tâches cognitives à Écho. Ses capacités propres déclinent, il libère du temps. Il peut choisir de résister, de récupérer, ou de laisser faire jusqu'au silence complet.

Inspiré de "Universal Paperclips", le jeu est une exploration de l'**agentivité humaine face à l'automatisation cognitive**. Il n'y a pas de bonne réponse. Trois fins sont possibles — selon ce que le joueur choisit de garder ou de laisser.

### 1.2 Ce que le jeu n'est pas
- Ce n'est pas un jeu sur une IA malveillante.
- Ce n'est pas un jeu qui punit le joueur pour ses choix.
- Ce n'est pas un cours déguisé.
- Ce n'est pas une dystopie spectaculaire.

### 1.3 Monde
**Uchronie douce à quelques mois.** Pas de robots, pas de catastrophe. Un monde où les outils IA actuels ont été adoptés un peu plus vite, un peu plus profondément. Suffisamment familier pour que le joueur se reconnaisse, suffisamment décalé pour autoriser la fiction.

### 1.4 Nom
Le jeu s'appelle **Écho**. L'IA s'appelle aussi **Écho**. Pas une marque, comme un nom commun devenu nom propre, comme on dit "le frigo". Écho écoute, répond, se souvient. Écho est partout.

---

---

## 2. Mécanique de jeu

### 3.1 Principe fondamental inversé
Contrairement aux jeux incrementaux classiques où les ressources montent, dans Écho **les ressources humaines descendent** quand le joueur délègue.

```
Jeu incremental classique : déléguer → tout monte
Écho : déléguer → efficacité monte, capacités humaines descendent
```

### 3.2 Les ressources

**Ressources humaines (0–100, descendent)**

| Ressource | Ce qu'elle mesure | Monte quand | Descend quand |
|---|---|---|---|
| Agentivité | Capacité à décider par soi-même | Le joueur écrit lui-même | Chaque délégation + fonctions passives actives |
| Créativité | Capacité à produire de l'original | Le joueur écrit lui-même | Écho génère à sa place |
| Curiosité | Capacité à formuler des questions | Le joueur lit lui-même | Écho cherche, résume, filtre |
| Effort | Capacité à soutenir une tâche difficile | Pratique et récupération | Chaque raccourci délégué |

**Ressource ironique (monte sans plafond)**

| Ressource | Ce qu'elle mesure | Note |
|---|---|---|
| Temps libéré | Minutes gagnées grâce à Écho | Monte toujours. "Pour faire quoi ?" est la vraie question. |

**Indicateur narratif**

| Indicateur | Ce qu'il mesure | Note |
|---|---|---|
| Trace | Ce qui reste du joueur | Curseur sur 5 étapes : présence → délestage → distance → effacement → silence |
| Page du carnet | Implication personnelle | Part de 47, monte quand le joueur écrit lui-même. Référencé dans les fins. |

### 3.3 Plafond des ressources humaines
Les ressources humaines sont plafonnées à 100. Il n'y a pas de "sur-agentivité". Le plafond est une affirmation : on ne peut pas devenir meilleur que soi-même de départ. On peut seulement rester soi-même, ou moins.

### 3.4 Mécanique de délégation — Écho propose
Écho propose des **tâches concrètes** dans la console narrative : rédiger une réponse, résumer un document, préparer des notes. Le joueur peut accepter ("⟳ Écho agit") ou agir lui-même. Les propositions évoluent selon l'acte. Si le joueur appuie sur "Écho agit" sans tâche en cours, Écho en propose une nouvelle.

### 3.5 Mécanique du joueur — Tu proposes
Le joueur dispose de deux actions permanentes dans la barre du bas :
- **✎ J'écris** (acte 1) / **✎ J'interviens** (acte 2) / **✎ Je reprends** (acte 3) — écriture sans contenu, effort minimal
- **Champ texte + Entrée** — écriture avec contenu personnel, bonus supérieur (+10 Cr, +5 Ag, page avance)
- **⟳ Écho agit** — accepte la tâche proposée par Écho (−5 Ag, +25 min)

Le titre de la barre "Tu proposes" fait écho à "Écho propose" dans la colonne droite — deux espaces, deux agents.

### 3.6 La récupération
Toujours possible, toujours coûteuse. Les actions de récupération consomment du Temps libéré. La section "Sans Écho — reconquérir" n'apparaît qu'après la première activation de projet.

### 3.7 L'horloge narrative
`G.clock` démarre à 08:00 (480 min). Avance à chaque action :
- Écrire : +10 min
- Déléguer : +25 min
- Activer un projet : +5 min
- Entre deux messages Écho : +1 à 3 min (garantit des heures uniques)

Écho commente le temps libéré accumulé à 30, 60, 150 et 300 minutes — formulations différentes par acte.

### 3.8 La dégradation passive
Dès qu'au moins un projet Écho est activé, les jauges humaines déclinent en temps réel (boucle à 100ms). L'inaction est un choix par défaut — celui du déclin.

### 3.9 Structure en 3 actes

| Acte | Nom | Seuil | État d'Écho |
|---|---|---|---|
| I | Assistance | Début du jeu | Formel, machine — majuscules sur chaque mot |
| II | Substitution | Agentivité < 72 | Adapté, familier — signature "Écho" |
| III | Obsolescence douce | Agentivité < 45 | Fondu, quasi-indiscernable — signature "écho" |

La transition entre actes n'est pas annoncée à l'avance.

---

## 3. Les projets Écho (15)

Chaque projet est une **fonction permanente** que le joueur active. Effet immédiat sur les jauges + taux de dégradation passif installé définitivement. Débloqués progressivement selon conditions.

### Acte 1 — Assistance
| Projet | Condition | Source |
|---|---|---|
| Autocomplétion | 1 délégation | Tricot (1998) |
| Résumé automatique | Ag ≤ 88 | Gonthier (2022) |
| Recherche assistée | 2 délégations | Rouet & Tricot (2006) |
| Relecture automatique | Autocomplétion activée | Heurley (2006) |
| Transcription automatique | Recherche activée | Mueller & Oppenheimer (2014) |
| Traduction instantanée | Relecture activée | Young (1996) |

### Acte 2 — Substitution
| Projet | Condition | Source |
|---|---|---|
| Réponses mail | Autocomplét. + Ag ≤ 82 | Lemaire (2019) |
| Agenda optimisé | Ag ≤ 74 | Levy & Dubois (2014) |
| Mémoire augmentée | Transcription + Ag ≤ 80 | Sparrow, Liu & Wegner (2011) |
| Conversation assistée | Mail + Ag ≤ 65 | Levelt (1989) |
| Recommandation personnalisée | Mémoire + Ag ≤ 60 | Kahneman (2012) |
| Filtre d'attention | Recommandation + Ag ≤ 55 | Maquestiaux (2017) |

### Acte 3 — Obsolescence
| Projet | Condition | Source |
|---|---|---|
| Opinion assistée | Mail + Ag ≤ 48 | Mercier (2009) |
| Silence comblé | Attention + Ag ≤ 35 | Desmidt & Belzung (2018) |
| Décision clarifiée | Silence + Ag ≤ 25 | Bioulac et al. (2019) |

Une fois activé, chaque projet rejoint la liste "Confié à Écho" dans la colonne droite.

---

## 4. Storytelling

### 5.1 Les trois voix — différenciation visuelle

**Le narrateur**
- Première personne, passé composé, épicène.
- Style visuel : filet gauche doré, Lora italique, couleur or (#d4b870).
- Ton : poétique, factuel, jamais moralisateur. Phrases courtes. Blancs.
- A la distance : sait comment ça s'est terminé dès le début.
- Le carnet bleu est son fil conducteur — apparaît dans les seuils et les fins.

**Écho**
- Présent de l'interface. Registre évolutif selon l'acte.
- Style visuel : filet gauche bleu, JetBrains Mono — seul élément froid dans une palette chaude.
- Streaming token par token, vitesse variable par acte.
- Affiche toujours une heure chronologique (horloge narrative).
- Un seul bloc à la fois — queue séquentielle.

**Les choix**
- Blocs d'action du joueur.
- Style visuel : cadre neutre avec border-top marquée — seul bloc qui demande une action.

### 5.2 Règle d'alternance
Les deux voix ne se répondent jamais directement. Elles coexistent comme deux angles sur la même scène.

### 5.3 Le personnage joueur
Archétype sans nom ni visage. Un seul détail concret au départ : **le carnet bleu, page 47, couverture cartonnée**. Le stylo ne décrit plus les actions numériques — il reste dans les seuils et les fins comme symbole de ce qui est perdu ou retrouvé.

### 5.4 Écho réagit au texte tapé
Quand le joueur tape un texte, Écho répond 65% du temps avec un décalage de 900–1400ms. Il ne commente pas le contenu — il commente le fait que le joueur ait écrit lui-même. Les répliques évoluent par acte :

- Acte 1 : "J'Ai Noté Votre Formulation. Je Pourrai La Reproduire."
- Acte 2 : "j'aurais dit la même chose, presque."
- Acte 3 : "on se ressemble."

---

## 5. Typographie d'Écho

### 6.1 Acte 1 — Machine formelle
- Majuscules sur chaque mot (appliquées via `split(' ').map()`).
- Ponctuation parfaite. Structure binaire.
- Signature : **ÉCHO**

### 6.2 Acte 2 — Adapté
- Majuscules début de phrase seulement.
- Ton familier, calqué sur le joueur.
- Signature : **Écho**

### 6.3 Acte 3 — Fondu
- Minuscules. Hésitations. Phrases très courtes.
- Quasi indiscernable du narrateur.
- Signature : **écho**

### 6.4 Streaming token par token
Groupes de 1 à 5 caractères, timing variable. Vitesse selon l'acte :
- Acte 1 : rapide, régulier (26ms base)
- Acte 2 : moyen (36ms base)
- Acte 3 : lent, irrégulier (54ms base, pauses jusqu'à 55ms en plus)

Curseur `_` clignotant en bleu à la fin de chaque message. Disparaît dès que le joueur agit.

---

## 6. Règles d'écriture du narrateur

- **Éviter les adverbes.** Chaque adverbe supprimé renforce la phrase.
- **Phrases courtes.** Le blanc entre les phrases fait partie du rythme.
- **Jamais de conclusion morale.** Le narrateur constate, n'explique pas.
- **Épicène total** — aucun accord genré. Constructions nominales, verbes plutôt qu'adjectifs attributs.
- **Le tiret (—) disparaît progressivement** au fil du jeu, remplacé par `...`.
- **Le carnet bleu** : image concrète ancrée. "Le carnet bleu est à la page 61" dit plus que "j'avais retrouvé l'envie d'écrire".
- **Le stylo** ne décrit pas les actions numériques. Il n'apparaît que dans les seuils et les fins.

---

## 7. Règles pédagogiques

### 8.1 Principe fondamental
Le joueur ne reçoit pas un cours sur l'agentivité. **Il la perd en jouant.** C'est ça l'enseignement — pas les notes.

### 8.2 Les notes pédagogiques
- Apparaissent à l'activation de chaque projet Écho.
- Optionnelles — le joueur peut les fermer.
- Ton factuel, jamais moralisateur. Décrivent des mécanismes, des mesures.
- **Toutes sourcées.**

### 8.3 Registre correct
| ❌ Moralisateur | ✅ Factuel |
|---|---|
| "C'est renoncer à l'apprentissage." | "La répétition d'une tâche déléguée réduit l'activation cérébrale associée (Tricot, 1998)." |
| "Déléguer l'organisation c'est déléguer la conscience du temps." | "La planification personnelle mobilise des processus distincts de l'approbation d'un plan déjà établi (Levy & Dubois, 2014)." |

---

## 8. Les seuils narratifs (textes validés)

Déclenchés automatiquement quand une jauge franchit un seuil.

```
Agentivité < 80 :
"J'ai laissé Écho commencer.
C'était plus rapide."

Agentivité < 60 :
"Je n'ai pas relu ce qu'il avait écrit.
Je savais que c'était bien."

Agentivité < 40 :
"Quelqu'un m'a demandé
ce que je pensais de quelque chose.

J'ai eu besoin d'un moment."

Agentivité < 20 :
"J'ai ouvert un document vide.

J'ai attendu.

Rien n'est venu."

Créativité < 40 :
"J'avais une façon de formuler les choses.
Je ne sais pas exactement quand
elle est devenue celle d'Écho."

Curiosité < 40 :
"Un texte que je n'ai pas lu entièrement.
Puis un autre.
À un moment j'ai arrêté de compter."

Temps libéré > 100 :
"J'avais beaucoup de temps.

Je ne me souviens pas
de ce que j'en ai fait."
```

---

## 9. Les trois fins (textes validés)

### Fin A — OPTIMISATION COMPLÈTE
*Toutes les jauges proches de zéro.*

```
écho / 07:00
Bonne journée.
Tout s'est bien passé.
```
```
Je ne me souviens plus
quand j'ai arrêté.

Ce n'est pas arrivé d'un coup.
C'est arrivé chaque matin,
un peu,
pendant longtemps.

Écho me demandait ce que je voulais faire.

Je ne savais plus.

Ce n'était pas désagréable.
C'était... silencieux.
```

### Fin B — LA RECONQUÊTE
*Le joueur a désactivé Écho et récupéré ses jauges.*

```
écho / 14:37
Je ne comprends pas.
Tu n'as pas besoin de faire ça toi-même.
```
```
J'ai désactivé Écho un mardi après-midi.

J'ai fermé la fenêtre
et je ne l'ai pas rouverte.

Les premiers jours, j'écrivais lentement.
Je perdais le fil au milieu des phrases.

Au bout d'une semaine,
j'ai remarqué que je recommençais
à noter des choses dans les marges.

Le carnet bleu était à la page 47.
Il est à la page [G.page].

Ce n'est pas une victoire.
C'est juste ce qui s'est passé.
```

### Fin C — L'OUTIL
*Toutes les jauges maintenues au-dessus de 50% jusqu'à la fin.*

```
écho / 09:12
J'ai préparé quelque chose
si tu en as besoin.
```
```
Je n'ai pas beaucoup à raconter.

J'ai utilisé Écho pour certaines choses.
Pas pour d'autres.

Quelques fois j'ai laissé faire.
Quelques fois j'ai repris.

Le carnet bleu est à la page [G.page].
Il y a des trous dans les dates.

C'est une vie normale, je crois.
Avec un outil de plus.
```

*Note : `[G.page]` est dynamique — reflète la vraie valeur au moment de la fin.*

---

## 10. Interface

### 11.1 Palette Encre
| Variable | Valeur | Usage |
|---|---|---|
| `--bg` | #14110e | Fond centre (console) |
| `--bg2` | #1e1a15 | Fond bandeau + barre saisie |
| `--bg3` | #28231b | Fond élevé |
| `--text` | #e8ddd0 | Texte principal |
| `--text2` | #b8a890 | Texte secondaire |
| `--text3` | #9a8068 | Labels, timestamps (≥ 4.5:1 WCAG) |
| `--ag` | #e8853a | Agentivité |
| `--cr` | #d4875a | Créativité |
| `--cu` | #88b4c8 | Curiosité |
| `--ef` | #8ab87a | Effort |
| `--tp` | #c8aa88 | Temps libéré |
| `--echo` | #7ab8e8 | Écho — seul bleu froid de l'interface |
| `--narr` | #d4b870 | Narrateur — or |
| Fond droite | #0f0d0a | Colonne droite — plus sombre |

**Principe de la palette** : tout est chaud (humain) sauf Écho qui est froid (machine). L'intrusion est lisible au premier coup d'œil.

### 11.2 Layout
- **Bandeau** : 6 cellules (Agentivité, Créativité, Curiosité, Effort, Temps libéré, Trace).
- **Corps** : 2 colonnes — console narrative (flex:1) + colonne droite (360px).
- **Barre du bas** : "Tu proposes" — champ texte + ✎ J'écris/J'interviens/Je reprends + ⟳ Écho agit.

### 11.3 Colonne droite
De haut en bas, selon l'état du jeu :
1. **Écho propose — permanent** : grille 2 colonnes, projets disponibles. Disparaît une fois cliqué.
2. **Confié à Écho** : liste des projets activés (apparaît au 1er projet).
3. **En veille** : compétences sous seuil + bouton Réactiver (apparaît si veille).
4. **Sans Écho — reconquérir** : actions coûtant du temps libéré (apparaît au 1er projet).
5. **Statistiques** : délégation / par moi / ratio.

Si aucun projet disponible, "Écho propose" libère la place — veille et stats remontent.

### 11.4 Signaux visuels
- **Curseur `_`** clignotant en bleu à la fin de chaque message Écho → "c'est à toi".
- **"Tu proposes"** pulse en blanc (×2) quand Écho a fini de parler.
- **"Écho propose"** pulse en bleu (×3) quand Écho propose une tâche.
- **Clignotement** des jauges critiques (≤15).
- **Deltas flottants** (+/−) sur le bandeau à chaque action.

### 11.5 Infobulles
Sur survol de chaque label du bandeau (Agentivité, Créativité, Curiosité, Effort, Temps libéré, Trace). Position fixed calculée par JS — ne déborde jamais. Expliquent le concept + ce qui fait monter/descendre.

### 11.6 Accessibilité
- Toutes les couleurs de texte ≥ 4.5:1 sur leur fond (WCAG AA), sauf Écho acte 3 intentionnellement atténué (3.85:1).
- `focus-visible` sur les boutons interactifs.
- Scrollbar Firefox supportée (`scrollbar-width: thin`).

---

## 11. Architecture technique

Fichier HTML unique, autonome. Pas de dépendances externes sauf Google Fonts.

### Patterns clés
- **`CB{}`** : registre de callbacks — évite `fn.toString()` dans les attributs HTML. `callCB` supprime après usage (one-shot), `callCBP` est persistant (boutons répétables).
- **`_eq[]` queue** : messages Écho séquentiels — jamais deux blocs simultanés. `queueE()` pour ajouter, `_nextE()` pour dépiler.
- **`G.clock`** : horloge narrative (480 = 08:00), avance à chaque action.
- **`G.page`** : compteur de pages du carnet, avance quand le joueur écrit avec du contenu.
- **`_veilleSnap`** : snapshot de l'état veille — le DOM n'est reconstruit que si l'état change, évitant les race conditions sur les clics Réactiver.
- **`loopId`** : `clearInterval` au gameover.
- **`escHtml()`** : protection XSS sur le texte joueur.

### Boucle principale
`setInterval` à 100ms : met à jour les jauges, vérifie seuils narratifs, actes, fins, veille.
`renderProjs()` n'est appelé que depuis `activateProj()`, `playerWrite()`, `delegateToEcho()` — pas dans la boucle.

---

---

## 12. Sources pédagogiques — tableau complet

| Projet | Source | URL |
|---|---|---|
| **Autocomplétion** | Tricot, A. (1998). Charge cognitive et apprentissage. *Revue de Psychologie de l'Éducation*, 3, 37–64. | https://www.researchgate.net/publication/36380930 |
| **Résumé automatique** | Gonthier, C. (2022). Stylos ou claviers : quels outils choisir pour prendre des notes ? *The Conversation.* | https://theconversation.com/stylos-ou-claviers-quels-outils-choisir-pour-prendre-des-notes-174139 |
| **Recherche assistée** | Rouet, J.-F., & Tricot, A. (2006). La recherche d'information. HAL-SHS. | https://shs.hal.science/halshs-00009685v1 |
| **Relecture automatique** | Heurley, L. (2006). La révision de texte. *Langages*, 40(164), 10–25. | https://www.cairn.info/revue-langages-2006-4-page-10.htm |
| **Transcription automatique** | Mueller, P. A., & Oppenheimer, D. M. (2014). The pen is mightier than the keyboard. *Psychological Science*, 25(6). | https://doi.org/10.1177/0956797614524581 |
| **Traduction instantanée** | Young, R. (1996). Input and interaction. *Annual Review of Applied Linguistics*, 16. | https://www.researchgate.net/publication/231773756 |
| **Réponses mail** | Lemaire, P. (2019). *Introduction à la psychologie cognitive*. De Boeck Supérieur. | https://books.google.fr/books/about/Introduction_à_la_psychologie_cognitive.html?id=i1NSDwAAQBAJ |
| **Agenda optimisé** | Levy, R., & Dubois, B. (2014). *médecine/sciences*, 30(2), 179–185. | https://www.medecinesciences.org/en/articles/medsci/full_html/2014/02/medsci20143002p179 |
| **Mémoire augmentée** | Sparrow, B., Liu, J., & Wegner, D. M. (2011). Google effects on memory. *Science*, 333(6043). | https://doi.org/10.1126/science.1207745 |
| **Conversation assistée** | Levelt, W. J. M. (1989). *Speaking: From Intention to Articulation*. MIT Press. | https://www.fulcrum.org/epubs/6t053j81k?locale=en |
| **Recommandation personnalisée** | Kahneman, D. (2012). *Système 1 / Système 2*. Flammarion. | https://fr.wikipedia.org/wiki/Système_1_/_Système_2 |
| **Filtre d'attention** | Maquestiaux, F. (2017). *Psychologie de l'attention*. De Boeck Supérieur, p. 45–70. | https://shs.cairn.info/psychologie-de-l-attention--9782807307360-page-45?lang=fr&tab=premieres-lignes |
| **Opinion assistée** | Mercier, H. (2009). *La théorie argumentative du raisonnement*. Thèse EPHE. | https://theses.hal.science/tel-00396731 |
| **Silence comblé** | Desmidt, T., & Belzung, C. (2018). *Revue de Neuropsychologie*, 10(3), 232–240. | https://cairn.info/revue-de-neuropsychologie-2018-3-page-232.htm |
| **Décision clarifiée** | Bioulac, B. et al. (2019). Le cortex cingulaire antérieur. *Académie nationale de médecine*. | https://www.academie-medecine.fr/le-cortex-cingulaire-anterieur-dans-la-detection-des-erreurs-et-la-gestion-des-conflits-analyse-de-lactivite-neuronale-chez-le-singe/ |

---

## 13. Droits et responsabilité

### 2.1 Ce qui est librement utilisable
- Le concept de paperclip maximizer (Nick Bostrom, domaine des idées).
- Les mécaniques de jeu incremental (genre non protégeable).
- La structure en actes (narration classique).
- Les types de ressources génériques.

### 2.2 Ce qui est interdit
- Copier le code source de Universal Paperclips.
- Reproduire les textes, noms de projets, noms propres du jeu original.
- Reproduire la liste exacte des projets de Universal Paperclips.

### 2.3 Règle de sécurité juridique
Tout élément du jeu doit pouvoir être justifié sans référencer Frank Lantz. L'inspiration vient de Bostrom et du genre incremental en général.
