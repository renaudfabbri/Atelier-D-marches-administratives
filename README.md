# Quiz « Mes démarches en France » — Guide de mise en ligne

Le fichier **`index.html`** est un quiz complet et autonome (rien à installer).
Une fois en ligne, les résultats (prénom, score, détail) remontent **automatiquement**
à **c.lapree@fjt-tarbes.fr**, sans que l'apprenant ait à écrire un e-mail.

> 💡 **Tout de suite utilisable :** même sans aucune configuration, le bouton
> **« Envoyer par e-mail »** sur l'écran de résultats fonctionne déjà : il ouvre la
> messagerie avec un message pré-rempli vers c.lapree@fjt-tarbes.fr. Les 3 étapes
> ci-dessous servent à rendre la remontée **100 % automatique** (recommandé).

---

## Étape 1 — Créer le formulaire Formspree (gratuit)

1. Aller sur **formspree.io** → **Sign up**, avec l'adresse **c.lapree@fjt-tarbes.fr**.
2. Cliquer **+ New Form**, nommer le formulaire (par exemple : `Quiz démarches BPI`).
3. Copier l'adresse fournie, de la forme : `https://formspree.io/f/xxxxxxxx`.

## Étape 2 — Coller cette adresse dans le quiz

1. Ouvrir **`index.html`** avec un éditeur de texte (Bloc-notes, TextEdit…).
2. Chercher la ligne :
   ```
   var ENDPOINT_URL = "COLLER_URL_FORMSPREE_ICI";
   ```
3. Remplacer `COLLER_URL_FORMSPREE_ICI` par l'adresse copiée à l'étape 1, puis enregistrer.
   Exemple : `var ENDPOINT_URL = "https://formspree.io/f/xxxxxxxx";`

## Étape 3 — Mettre en ligne sur GitHub Pages

1. Créer un dépôt GitHub (par exemple `quiz-demarches`).
2. Déposer le fichier **à la racine du dépôt**. Le nom doit **obligatoirement** rester
   **`index.html`** (sinon la page affiche une erreur 404).
3. Aller dans **Settings ▸ Pages ▸ Source** : branche **`main`**, dossier **`/ (root)`**, puis **Save**.
4. Attendre environ 1 minute : un lien public apparaît (à partager ou à ouvrir sur la tablette).

## Étape 4 — ⚠️ Activation Formspree (à ne pas oublier)

À la **toute première vraie réponse envoyée**, Formspree adresse un **e-mail d'activation**
à c.lapree@fjt-tarbes.fr. **Cliquer sur le lien de confirmation** dans cet e-mail.
Sans cette confirmation, les réponses suivantes sont bloquées.

> Astuce : faites un premier essai vous-même après la mise en ligne, puis confirmez
> l'e-mail d'activation. Tout sera ensuite automatique pour les apprenants.

---

## Comment ça se passe pendant l'atelier

- Le quiz comporte **20 questions** de **difficulté progressive** : d'abord reconnaître les
  organismes (réponses en images), puis lire un papier (numéro, montant, date), puis les
  obligations, et enfin de petits scénarios. Conçu pour un **niveau A1** (phrases simples).
- La **page d'accueil** affiche une illustration d'accueil au guichet et demande le **prénom**.
- **L'animateur·rice peut lire chaque question à voix haute** (un rappel apparaît à l'écran)
  et saisir le prénom à la place de l'apprenant si besoin.
- Après chaque réponse : un **retour immédiat** (✅ / ❌) avec une courte explication.
- À la fin : le **score** s'affiche et le résultat part **automatiquement** vers
  c.lapree@fjt-tarbes.fr (et apparaît dans le tableau de bord Formspree, une ligne par apprenant).

## Où retrouver les résultats

- Dans la **boîte mail** c.lapree@fjt-tarbes.fr (une notification par participation).
- Dans le **tableau de bord Formspree** (onglet *Submissions*) : prénom, score, pourcentage
  et le détail question par question (OK / raté).
