# EVOL — Éditeur de newsletter

Un seul fichier : **`index.html`**. Double-cliquez dessus : il s'ouvre dans votre navigateur (Chrome, Edge, Safari, Firefox). Aucune installation, aucun compte à créer.

## 1. Écrire la newsletter

- **Colonne de gauche** : tous les textes, classés en 7 panneaux (image d'en-tête, titre, introduction, blocs 01/02, signature, pied de page).
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

## Aide-mémoire des limites

| Élément | Limite |
|---|---|
| Plan gratuit Brevo | 300 e-mails / jour |
| Recommandé | ~100 contacts = aucun problème |
| Photos importées | stockées dans le navigateur (évitez les fichiers > 5 Mo) |

En cas de doute : faites d'abord **Envoyer un test**, toujours.
