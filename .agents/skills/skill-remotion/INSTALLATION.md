# Skill Remotion pour Sahla

## Provenance

Source officielle : https://github.com/remotion-dev/skills
Commit importé : `6c67adcd9cdbe6eb84d76342da89b225f9161cb2`
Dossier source : `skills/remotion-best-practices` (version déclarée 4.0.538).

Le dossier complet a été conservé avec ses références, exemples, scripts et icônes.
Seuls le nom et la description dans SKILL.md et les mentions du nom dans
agents/openai.yaml ont été adaptés à `skill-remotion`.
Ce dossier contient une skill d'instructions, pas le code source du moteur Remotion.

## Utilisation dans Codex

Ouvrir ce dépôt comme projet dans Codex. Si la conversation existait avant
l'installation, démarrer une nouvelle conversation dans ce projet pour recharger
les skills. Aucune modification de la configuration globale n'est nécessaire.

Exemple :

> Utilise $skill-remotion pour créer un Reel publicitaire vertical de 15 secondes
> pour mon produit. Prépare une composition Remotion et son aperçu.

Autres demandes possibles : améliorer une animation, ajouter des sous-titres,
préparer une démonstration de site à partir de captures fournies, puis demander
explicitement l'export MP4 quand le résultat convient.

Lire SKILL.md, puis remotion-create/REFERENCE.md pour une nouvelle vidéo,
remotion-markup/REFERENCE.md pour les animations et
remotion-render/REFERENCE.md pour un export explicite.

## Dépendances

La découverte de la skill ne nécessite aucune installation npm. Les scripts et
exemples sont des ressources à utiliser selon la tâche, pas des services à démarrer.
Le projet vidéo aura besoin de Node.js, de ses dépendances Remotion et de celles
indiquées par les références utilisées. Aucun projet vidéo n'a été créé par cette
installation. Les captures de sites, médias, voix et services externes nécessitent
leurs propres outils et éventuels accès ; la skill ne les fournit pas à elle seule.

## Vérifications réalisées

- Codex CLI : appel réel `skills/list` pour ce dépôt, via un serveur éphémère
  et un CODEX_HOME temporaire, sans modifier la configuration Codex existante.
- Résultat : `skill-remotion`, scope `repo`, `enabled: true`, aucune erreur.
- Les 139 références Markdown locales de la distribution importée existent.
- Aucun rendu vidéo ou accès à un service multimédia externe n'a été testé.

## Mise à jour

Ne pas lancer une réinstallation générique qui créerait une deuxième skill sous
un autre nom. Comparer une future version officielle à ce dossier et conserver
le nom `skill-remotion`, ses chemins relatifs et les éventuelles adaptations locales.
