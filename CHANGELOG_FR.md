# Changelog — Axovox

Toutes les versions notables d'Axovox sont documentées ici.
Notes de version complètes : [GitHub releases](https://github.com/Sebastien-VZN/axovox/releases)

---

## [beta_0.14.1] — 2026-08-21

- Correctifs du workflow GitHub après le renommage AuroriaLink → Axovox
- Correctifs de gestion du token CI et de tests

## [beta_0.14.0] — 2026-08-21

Période : mai 2026 à août 2026 — 44 commits, 466 fichiers modifiés.

### Nouveau nom : Axovox (anciennement AuroriaLink)
- Renommage complet en « Axovox » — plus court, mémorable, aligné avec l'écosystème Axomind
- Même produit, même base de code, nouvelle identité sur l'app, le CI/CD, le dépôt GitHub et la documentation

### Correcteur orthographique natif — migration vers la correction OS
- Remplacement de l'ancien correcteur maison (`GstSpellCheck`, 363 lignes) par notre fork `native_spell_checker`, publié sur GitHub
- Utilise le correcteur orthographique de l'OS directement : WinRT `ISpellChecker2` sur Windows, `libhunspell-1.7` sur Linux, `DefaultSpellCheckService` de Flutter sur Android
- Zéro dictionnaire embarqué — l'OS fournit tout
- `SpellCheckTextFormField` comme remplacement direct de `TextFormField`
- 100% hors-ligne, aucune API cloud

### 33 langues avec drapeaux natifs
- Traduction complète de l'interface en 33 langues, drapeau dédié pour chaque langue

### 27 thèmes avec variantes claire et sombre
- Chaque thème propose des variantes claire et sombre
- Couleurs extraites vers le package partagé `quodexus_color` (7 139 lignes retirées de l'app, désormais maintenues comme dépendance autonome)
- Animations de fond : Aurora, particules, cyberpunk et terminal retro
- Effets de glassmorphisme via `BackdropFilter` et `ImageFilter.blur` dans toute l'interface

### Système de quotas (reconstruit)
- Reconstruction complète de la gestion des quotas côté client
- Trois plans d'abonnement : free, perso et pro
- Limites par plan sur la durée d'enregistrement audio, la taille des fichiers, les uploads simultanés et plus

### Messagerie
- Mise à jour majeure de la messagerie avec amélioration de la stabilité
- Correction d'un plantage aléatoire d'une instance dans le module de messagerie
- Amélioration du défilement et du positionnement dans les conversations

### Éditeur de texte riche
- Corrections de stabilité et de défilement sur TextAreaEditor et TextAreaViewerStatic
- Migration vers le shared core pour une meilleure maintenabilité

### Mobile et UX
- Correction des performances des animations sur mobile
- Correction du sélecteur de fichiers
- Plusieurs corrections de build et configuration Android

### Infrastructure
- **Pipeline CI/CD entièrement réécrit** : job `validate` (format, analyse statique, tests unitaires et d'intégration), `android-build`, `linux-build`, `windows-build`, job `release` avec checksums SHA256 publiés sur Forgejo et GitHub
- Flutter 3.47.1 (Dart 3.13.1) version fixée sur tous les jobs
- Flutter, Dart SDK et Android Gradle Plugin mis à jour vers la dernière version stable
- Shared core migré vers une architecture de package partagé
- 593 tests dans 53 fichiers (core : 193, models : 55, network : 62, security : 24, intégration : 259)

## [beta_0.11.0] — 2026-07-07

### Améliorations
- **Notifications Android refondues** — reconstruites sur l'API native Android, plus de conflits de permissions
- **Démarrage plus stable** — préférences utilisateur et données de session chargées au bon moment du cycle de démarrage, évitant des crashs occasionnels

### Corrections
- **Crash aléatoire dans la messagerie** — instance provoquant un plantage intermittent corrigée
- **Build Android** — Gradle et Kotlin mis à jour pour les derniers SDK Android
- **Lecteur de fichiers** — meilleure gestion des fichiers médias partagés dans les conversations

### Technique
- Mise à jour des dépendances Flutter
- CI/CD migré vers une infrastructure plus robuste

## [beta_0.10.5] — 2026-05-26

- Corrections de stabilité et ajustements internes
- Mise à jour des dépendances du projet

## [beta_0.10.4] — 2026-05-13

### Messagerie
- Mise à jour majeure : meilleures performances, correction d'un crash aléatoire et affichage amélioré sur les téléphones en basse résolution

### Sécurité
- Meilleure gestion des sessions : déconnexion plus propre

### Traductions
- Textes français et anglais mis à jour et étendus

## [beta_0.10.3] — 2026-05-13

- Premier déploiement de la mise à jour majeure de la messagerie — performance, stabilité et affichage basse résolution (stabilisée dans la beta_0.10.4)

## [beta_0.10.1] — 2026-05-10

### Mise à jour majeure
- **Gestion des droits étendue sur les groupes** — deux niveaux d'accès : participants en lecture (lecture des messages) et participants en écriture (envoi + modification des paramètres) ; seul le créateur du groupe gère les bots et les droits complets
- **Messagerie améliorée** — interface plus fluide sur les longues conversations, meilleur défilement, détection automatique des URLs améliorée, conversion automatique des longs messages en fichiers Markdown, navigation et animations retravaillées
- **Performances globales** — optimisation du rendu, meilleure gestion de la mémoire lors des uploads et changements de page, démarrage plus rapide et plus stable
- **Correcteur orthographique enrichi** — dictionnaires FR/EN nettement plus complets, meilleure détection des élisions et mots composés, ignore automatiquement URLs/emails/mentions/hashtags, suggestions plus pertinentes
- **Stabilité** — nombreux correctifs de connexion/déconnexion, meilleure résilience en cas de perte de connexion
- **Divers** — gestionnaires de médias et fichiers améliorés, intégration des bots plus fiable, synchronisation temps réel renforcée

## [beta_0.10.0] — 2026-05-10

- Migration globale du code depuis la base Axomind vers le dépôt AuroriaLink
- Documentation, lint et correctifs internes

## [beta_0.9.0] — 2026-03-17

### Correcteur orthographique intégré
- Nouveau correcteur local intégré directement à la messagerie (français + anglais)
- Smart Check : élisions françaises, mots composés, filtrage automatique des URLs, emails, mentions et hashtags
- Suggestions Levenshtein avec cache ; sur mobile, correcteur natif du clavier utilisé par défaut

### Messagerie repensée
- Refonte majeure de la messagerie : interface plus fluide et logique centralisée
- Correction du comportement du scroll et de la position de conversation
- Amélioration des animations et de l'UX générale

### Stabilité et performances
- Refonte de la gestion async : UI plus robuste, moins de gels et de comportements inattendus
- Démarrage de l'app plus rapide et plus fiable

## [beta_0.8.4] — 2026-03-03

- Messages désormais conservés 6 mois (au lieu de 15 jours) ; fichiers non épinglés conservés 1 mois
- Durée de vie des conversations correctement sauvegardée (un changement de durée ne s'appliquait parfois qu'après une restauration)
- Améliorations visuelles mineures dans le chat ; composants Android internes mis à jour ; plusieurs bugs mineurs corrigés

## [beta_0.8.3] — 2026-02-10

- Ajustement de la configuration WebSocket pour éviter de rares interruptions de service

## [beta_0.8.2] — 2026-02-03

- Système audio unifié (`GstAudio`) centralisant la lecture et la gestion du volume utilisateur
- Prévisualisation des sons de notification (`MiniPlayerWidget`) directement depuis les paramètres
- `notification_locale` refactoré sur la nouvelle implémentation `GstAudio`
- Parsing JSON plus strict avec logs de débogage enrichis
- Ajustements UI : centrage des boutons et épaisseur des bordures harmonisée

## [beta_0.8.1] — 2026-01-29

- Correctifs d'UX dans la messagerie, notamment le défilement des conversations

## [beta_0.8.0] — 2026-01-27

- Intégration complète de l'API des bots — les bots envoient des messages directement dans les conversations (`GstDataBots`)
- Moteur de recherche intégré pour retrouver rapidement messages et documents
- Blocage d'utilisateurs (liste locale synchronisée avec le serveur)
- Système de thèmes harmonisé : 16 thèmes (Aurora, Axomind, Forest…) en modes clair et sombre
- Indicateurs visuels pour les nouveaux messages dans les threads ; correctifs ergonomiques mobiles (player audio, navigation Android)
- Amélioration des mises à jour temps réel WebSocket (bots et statuts) ; clarification de la séparation des modules Axomind / AuroriaLink

## [beta_0.7.2] — 2026-01-20

- Correctif mineur de l'UX

## [beta_0.7.1] — 2026-01-19

- 5 nouveaux thèmes : Biohazard, Dracula, Nebula, Retro Term 70 Red, Synthwave (variantes clair + sombre)
- Correction des mises à jour temps réel des bots via WebSocket ; amélioration de la gestion des états et de l'affectation des bots
- Correctifs : formulaire de focus group, page de gestion des bots, formatage des dates
- Côté serveur : correctif de sécurité sur la gestion des tokens d'échange, renforcement de la validation d'authentification

## [beta_0.7.0] — 2026-01-17

- Framework Bot API : authentification par tokens chiffrés, API dédiée d'envoi de messages, interface de gestion dans le dashboard, distinction visuelle bots/humains
- Chaînes de cryptage étendues

## [beta_0.6.0] — 2025-12-31

- Marquage visuel (ligne de séparation verte) avant les nouveaux messages non lus, dans le respect des groupes de messages
- Compteurs intelligents de non-lus (incrémentaux, reset après 10s ou au focus de la fenêtre)
- Intégration desktop : icône de notification dans le systray et badge de comptage dans la barre des tâches
- Mises à jour WebSocket optimisées sans redessiner toute la liste de conversation

## [alpha_0.5.5] — 2025-12-30

- Module audio : correctifs de stabilité de lecture, gestion mémoire des gros fichiers, support Debian 13

## [alpha_0.5.4] — 2025-12-19

- Ajout du copier dans la messagerie

## [alpha_0.5.3] — 2025-12-19

- Correctif sur la détection des URLs

## [alpha_0.5.2] — 2025-12-18

- System tray desktop (Windows) avec icône de notification, compression des assets, refonte technique du messenger (mixins, gestion des formulaires)

## [alpha_0.5.1] — 2025-12-11

- 21 thèmes (clair + sombre), 8 fonds de chat, raccourci d'envoi personnalisable (Entrée / Ctrl+Entrée), interface modernisée

## [alpha_0.5.0] — 2025-12-03

- Premier déploiement 0.5.x — sortie du système de thèmes (notes détaillées publiées avec alpha_0.5.1)

## [alpha_0.4.0] — 2025-12-03

- Refonte structurelle majeure : moteur de navigation refondu + barre inférieure mobile, antivirus côté serveur et contrôle d'intégrité des fichiers, nouvelle base de données locale pour un chargement quasi instantané des conversations, set d'icônes unifié, optimisations mémoire

## [alpha_0.3.0] — 2025-11-23

- Raffinement de l'interface (bordures, contrastes, états de survol), détection intelligente des URLs dans l'éditeur, nouveaux sons de notification + option muet, fiabilisation WebSocket, correctif de pagination des dashboards

## [alpha_0.2.0] — 2025-11-14

- Agrégateur d'emails centralisé, accès serveur externalisés, correctifs de sécurité et d'UX — base de données réinitialisée (comptes à recréer)

## [alpha_0.1.1] — 2025-11-11

- Upload de fichiers plus sûr avec validation automatique, taille de fenêtre minimale sur desktop, connexion instantanée après inscription, nombreux correctifs de bugs

## [alpha_0.1.0] — 2025-11-04

- Stabilisation : connexions PDO persistantes, optimisation des index PostgreSQL, cache de fichiers à 3 niveaux (APCu + ramdisk + Redis), charge CPU de déchiffrement réduite de 80%, heartbeat WebSocket, fermeture de session multi-appareils

## [alpha_0.0.6] — 2025-10-30

- Ajout des réactions + correctifs UX

## [alpha_0.0.5] — 2025-10-28

- Option de durée de vie des messages (24h / 3 mois), optimisation du WebSocket

## [alpha_0.0.4] — 2025-10-24

- Correctif WebSocket et amélioration de la synchro, correctif des touches de retour, notifications push

## [alpha_0.0.3] — 2025-10-21

- Correctifs d'instabilité et de pertes de références, guide visuel utilisateur, amélioration de la gestion des fichiers et des ressources

## [alpha_0.0.2] — 2025-10-14

- Correctifs : comptage des messages, ouverture de l'interface et gestion des groupes

## [alpha_0.0.1] — 2025-10-13

- Première alpha publique — ajout de la traduction
