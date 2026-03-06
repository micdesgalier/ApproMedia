# 📄 Rapport de Fin de Projet : Autoformation Cybersécurité (Réseau & Linux)

**Candidat :** Desgalier Michaël  
**Objectif :** Préparation aux Sélections Cybersoldat de l'Armée Suisse

---

## 1. Retour sur l'état initial et l'expérimentation

**Bilan entre attentes, objectifs et réalité :**

Au début de ce projet, mon but était de rattraper mon retard en infrastructure réseau pour être prêt pour les sélections des Cybersoldats. Je voulais réussir les modules Réseau et Linux de l'armée en obtenant au moins 70% de bonnes réponses aux examens.

Dans la pratique, mon expérience de développeur m'a énormément aidé. Pour la partie Linux, j'ai appris très vite à utiliser les commandes et à comprendre le système. En revanche, la partie Réseau m'a demandé beaucoup plus d'efforts pour mémoriser la théorie et comprendre les calculs d'adresses IP. Malgré cette différence de difficulté, j'ai réussi à atteindre et même dépasser mes objectifs sur la plateforme d'apprentissage.

---

## 2. Réponses aux 5 questions de contrôle

Voici les réponses expliquées avec mes propres mots :

### Q1 - Réseau : Différence entre TCP et UDP

* **TCP :** C'est un protocole fiable. Il vérifie que chaque donnée envoyée est bien arrivée dans le bon ordre. On l'utilise pour naviguer sur le web ou envoyer des fichiers, car on ne peut pas se permettre de perdre des morceaux en route.
* **UDP :** C'est un protocole très rapide, mais sans garantie de réception. Il envoie les données directement sans faire de vérifications. On l'utilise pour regarder des vidéos en direct, passer des appels ou jouer en ligne, car la vitesse est plus importante que la perte de quelques petites données.

### Q2 - Réseau : Calcul de réseau et de broadcast

Avec l'adresse IP 192.168.1.50 et un masque /26 (qui découpe le réseau en blocs de 64 adresses), on se trouve dans le tout premier bloc.
* **Adresse du réseau :** 192.168.1.0 (c'est le début du bloc).
* **Adresse de broadcast (diffusion) :** 192.168.1.63 (c'est la fin du bloc).

### Q3 - Linux : Gérer les permissions

Pour donner tous les droits au propriétaire (valeur 7), seulement lire et exécuter pour le groupe (valeur 5), et aucun droit pour les autres (valeur 0), la commande est :

chmod 750 script.sh

### Q4 - Linux : Chercher dans les historiques (logs)

Pour trouver le mot "Failed" dans le fichier des connexions et compter combien de fois il y est, on combine deux commandes :

grep "Failed" /var/log/auth.log | wc -l

### Q5 - Transversal : Voir les ports ouverts

Pour vérifier quels ports sont ouverts et prêts à recevoir des connexions sur ma machine, la commande la plus directe est :

ss -tuln

---

## 3. Investissement en temps

J'ai bien respecté les 36 heures prévues, mais j'ai un peu adapté mon planning en cours de route :

* **Linux :** J'ai passé moins de temps que prévu sur cette partie. Ma logique de programmeur m'a fait gagner beaucoup de temps pour comprendre les scripts et les commandes.
* **Réseau :** J'ai réutilisé le temps gagné sur Linux pour m'entraîner davantage sur le réseau. Les calculs de sous-réseaux m'ont demandé pas mal d'exercices pratiques pour être bien assimilés.
* **Organisation :** Les 6 heures de marge que j'avais prévues ont été très utiles pour comprendre comment utiliser la machine virtuelle, réviser et passer les examens en ligne.

---

## 4. Réflexion sur l'auto-formation

### Ce qui a bien marché :

* **La souplesse :** J'ai pu avancer très vite sur ce que je comprenais facilement et ralentir sur les concepts plus durs à digérer.
* **L'autonomie :** Quand je bloquais, j'ai dû chercher des solutions par moi-même (sur des forums ou dans la documentation). C'est une excellente habitude à prendre pour travailler dans la cybersécurité.

### Ce qui était plus compliqué :

* **Le risque de rester coincé :** Sans professeur pour corriger mes erreurs tout de suite, j'ai parfois perdu du temps à comprendre certains mécanismes réseau.
* **Le manque de matériel :** Apprendre le réseau sur un écran ne remplace pas la manipulation de vrais câbles, switchs et routeurs physiques.

---

## 5. Conclusion

Ce projet d'autoformation est une vraie réussite pour moi. J'ai bien compris qu'en cybersécurité, savoir coder ne suffit pas : il faut aussi comprendre comment les ordinateurs discutent entre eux sur un réseau. Ces 36 heures d'apprentissage ont renforcé ma motivation à devenir Cybersoldat. Aujourd'hui, je ne connais plus seulement la théorie ; je sais manipuler ces outils. Je me sens prêt et confiant pour affronter les sélections de l'armée suisse.
