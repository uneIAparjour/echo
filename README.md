# Écho
**Version :** 0.9.0

**Écran d'ouverture :** [uneiaparjour.github.io/echo/](https://uneiaparjour.github.io/echo/)

**Jouer directement :** [uneiaparjour.github.io/echo/echo.html](https://uneiaparjour.github.io/echo/echo.html)

**Mode facilitation :** [uneiaparjour.github.io/echo/echo.html?fac=1](https://uneiaparjour.github.io/echo/echo.html?fac=1)


---

Vous êtes à la page 47 d'un carnet bleu. Écho arrive et propose de corriger vos textes, résumer vos documents, répondre à vos mails, gérer votre agenda, compléter vos phrases. Chaque délégation libère du temps. Chaque délégation coûte un peu.

Le jeu dure vingt à trente minutes. Il n'y a pas d'ennemis, pas de score, pas de bonne réponse. Vous ne voyez pas quand Écho change. C'est souvent comme ça, on ne bascule pas, on glisse.

---

## Fichiers

| Fichier | Description |
|---|---|
| `index.html` | Page d'ouverture |
| `echo.html` | Le jeu, fichier unique autonome |
| `echo-regles.md` | Document de conception complet |
| `LICENSE.txt` | Licence CC BY-NC 4.0 |

→ [Règles de conception complètes](echo-regles.md)

---

## Public

Écho s'adresse à tout public. Aucune connaissance technique n'est requise.

Une utilisation en contexte éducatif est possible via le mode facilitation et le jeu cite des travaux de recherche en psychologie cognitive et neurosciences (Tricot, Maquestiaux, Sparrow, Kahneman et al.). Ce mode et ces sources peuvent servir de point de départ à une discussion sur la délégation cognitive aux outils d'IA.

---

## Utilisation avancée

### Mode facilitation

Destiné aux animateurs qui souhaitent piloter une démonstration en formation. Accessible via :

```
echo.html?fac=1
```

Un panneau de contrôle apparaît en bas de l'écran. Il permet de forcer les transitions d'actes, manipuler les jauges, déclencher des seuils narratifs, activer des projets sans conditions, et afficher les trois fins directement. Un bouton reset repart de zéro sans recharger la page. Le panneau est invisible pour les joueurs qui accèdent au jeu sans ce paramètre.

Le lien est accessible depuis la page d'ouverture.

### Intégration en iframe

Les deux fichiers sont intégrables indépendamment.

**Le jeu seul** (`echo.html`) :
```html
<iframe
  src="https://uneiaparjour.github.io/echo/echo.html"
  width="100%"
  style="border:none;height:700px;display:block"
  title="Écho — jeu narratif"
></iframe>
```

**La page de présentation** (`index.html`), si on souhaite proposer le contexte avant d'entrer dans le jeu :
```html
<iframe
  src="https://uneiaparjour.github.io/echo/"
  width="100%"
  style="border:none;height:700px;display:block"
  title="Écho"
></iframe>
```

**Dimensions recommandées :** 1100 × 700 px minimum. En dessous de 900 px de largeur, le jeu bascule automatiquement en version mobile.

### Sauvegarde

Le jeu ne sauvegarde pas les parties. C'est un choix intentionnel : fermer la fenêtre efface tout. La durée courte (20–30 min) rend la reprise peu nécessaire, et l'absence de sauvegarde renforce le propos — on ne revient pas en arrière.

---

## Licence

[CC BY-NC 4.0](LICENSE.txt) — Bertrand Formet, [uneIAparjour.fr](https://uneIAparjour.fr)

Vous pouvez partager et adapter ce travail librement à des fins non commerciales, à condition de créditer l'auteur.
