# EVOL — Éditeur de newsletter

Un seul fichier : **`index.html`**. Double-cliquez dessus : il s'ouvre dans votre navigateur (Chrome, Edge, Safari, Firefox). Aucune installation, aucun compte à créer.

## 1. Écrire la newsletter

- **Colonne de gauche** : tous les textes, classés en 9 panneaux (image d'en-tête, titre, introduction, blocs 01/02, blocs dynamiques, signature, apparence, options).
- Tout est **enregistré automatiquement** dans le navigateur (« Enregistré » en haut).
- **Mise en forme** dans les zones de texte :
  - `**texte en gras**` → **texte en gras**
  - `*texte en italique*` → *texte en italique*
  - `[voir la page](https://exemple.fr)` → lien cliquable
- **Aperçu à droite** : il se met à jour pendant que vous tapez. Bouton **Mobile** pour vérifier le rendu sur téléphone.
- **Redimensionner l'aperçu** : glissez la fine barre verticale entre l'éditeur et l'aperçu (double-clic dessus pour revenir à la taille par défaut). Sur un écran étroit, l'aperçu passe sous l'éditeur et reste collé à l'écran pendant que vous remplissez les formulaires.

## 2. Changer la photo d'en-tête

1. Panneau **01 — Le paysage**.
2. Cliquez **Importer une photo…** et choisissez une image de votre ordinateur (format paysage, idéalement 1200 px de large ou plus).
3. Vous pouvez aussi coller l'adresse web d'une image (URL), ou rétablir la **photo par défaut**.

> Pour l'envoi par e-mail, une photo importée depuis votre ordinateur est intégrée dans le fichier exporté, mais certains logiciels de messagerie bloquent les images « embarquées ». Pour un rendu garanti chez tous les destinataires, hébergez d'abord l'image (par exemple sur Google Drive en mode « partagé publiquement », puis copiez l'adresse du fichier) et collez cette adresse dans le champ URL.

## 3. Envoyer à vos contacts

Cliquez **Envoyer** (en haut à droite) :

1. **Expéditeur** : votre nom et votre e-mail (doit être validé une fois dans Brevo : *Expéditeurs & IP*).
2. **Objet** de l'e-mail.
3. **Contacts** : un par ligne — `Marie Dupont, marie@exemple.fr` ou simplement `marie@exemple.fr`. Les doublons sont ignorés automatiquement.
4. **E-mail de test** : recevez d'abord l'e-mail sur votre propre adresse pour vérifier le rendu.
5. **Clé API Brevo** (la première fois) :
   - Créez un compte gratuit sur [brevo.com](https://www.brevo.com) (300 e-mails/jour offerts).
   - Validez votre e-mail d'expéditeur dans Brevo (*Expéditeurs & IP*).
   - Copiez votre clé API (*SMTP & API → Clés API → Générer une nouvelle clé*) et collez-la dans le champ. Elle reste enregistrée dans votre navigateur.
   - Dès que la clé est en place, l'outil vérifie tout seul que l'expéditeur est validé : un encadré vert confirme, un encadré orange vous propose de choisir un expéditeur déjà validé en un clic. Sans cela, Brevo rejette l'envoi (« sender not valid »).
6. **Envoyer un test** → vérifiez votre boîte → **Passer à l'envoi** → confirmez.

L'envoi se fait par lots avec une barre de progression ; si une adresse échoue, elle est signalée individuellement à la fin.

## 4. Personnaliser les prénoms (optionnel)

Panneau **07 — Personnalisation avancée** : cochez la case et chaque contact dont la ligne contient un prénom (`Marie Dupont, marie@…`) recevra « Bonjour Marie, » au lieu de « Bonjour, ». L'envoi est alors un peu plus lent (un appel par contact), c'est normal.

## 5. Sauvegardes et export

- **Sauvegarde** (en haut) : télécharge un fichier `.json` de votre brouillon — à conserver ou à transmettre à un collègue.
- **Importer** : recharge un `.json` sauvegardé.
- **Exporter l'e-mail** : télécharge le HTML final, importable dans Brevo, Mailchimp, Gmail (via un outil comme « Templates ») ou tout autre outil d'envoi — utile si vous préférez passer par un autre service.

## Les blocs dynamiques (panneau 06)

Certaines éditions demandent d'annoncer un événement, lister des dates ou célébrer une réussite. Le panneau **06 — Les blocs dynamiques** permet d'ajouter autant de blocs que nécessaire, dans l'ordre voulu :

- **+ Événement** — titre, détails, photo à côté du texte, bouton de réservation optionnel.
- **+ Dates importantes** — une liste épurée « Date | description » (une ligne par date).
- **+ Win (photo / vidéo)** — un encadré doux pour célébrer une réussite, avec photo ou vidéo.
- **+ Paragraphe** — du texte libre, avec photo ou vidéo si besoin.

Chaque bloc se déplace (↑ ↓), se déplie en cliquant sur son en-tête et se supprime (✕). Tout est enregistré automatiquement.

**Photos et vidéos** :
- **Photo** : collez l'adresse (URL) d'une image en ligne (voir §2 pour l'héberger).
- **Vidéo YouTube / Vimeo** : collez simplement le lien de la vidéo — les e-mails ne peuvent pas lire de vidéo directement, donc l'outil insère automatiquement **la miniature de la vidéo avec un bouton de lecture** : le destinataire clique et la vidéo s'ouvre.

Les blocs sont insérés dans la lettre **après le bloc 01**, dans l'ordre affiché. Un bloc laissé vide n'apparaît pas dans l'e-mail : vous n'utilisez que ce dont l'édition a besoin.

## Les ambiances de couleur (panneau 08)

- **Nuit épurée** — noir profond neutre, textes clairs.
- **Ardoise** — gris-bleu profond et doux.
- **Ivoire** — clair et chaleureux.
- **Craie** — blanc pur, sobre.
- **Personnalisé** — la couleur de votre choix via la pastille de couleur.

Sur les thèmes clairs (Ivoire, Craie, personnalisé clair), le texte au-dessus de la photo reste **blanc** et le voile devient **sombre et discret** : le titre reste lisible même sur une photo sombre, tandis que la lettre garde des textes foncés très confortables à lire. La photo et le fond s'étendent sur toute la largeur de l'e-mail — aucune barre latérale. L'arrondi du bouton se règle au curseur (0 à 30 px, arrondi doux par défaut).

## Aide-mémoire des limites

| Élément | Limite |
|---|---|
| Plan gratuit Brevo | 300 e-mails / jour |
| Recommandé | ~100 contacts = aucun problème |
| Photos importées | stockées dans le navigateur (évitez les fichiers > 5 Mo) |

En cas de doute : faites d'abord **Envoyer un test**, toujours.
