#  Architecture de l'Administration (Maquette)

Ce document définit la structure globale et l'organisation des fichiers pour la maquette statique de l'administration SoliCode.

##  Organisation des Dossiers

```bash
maquette/
│
├── dashboard-admin.html    # Dashboard Admin complete
│
├── components/             # Briques Réutilisables
│   ├── KPI Cards/          # Cartes de statistiques
│   ├── Navbar/             # Barre supérieure
│   ├── Side-bar/           # Menu de navigation
│   ├── Activity List/      # Flux d'activités
│   └── Recent Articles/      # Composants de formulaire
│
└── prompts/                # Prompts
    ├── 00-architecture.md  # (architecture dashboard admin)
    ├── 01-generator-prompt.md 
    └── 02-dashboard-admin.md 
```

##  Principes de Développement

1. **Modularité Statique** : Chaque élément visuel est un fragment HTML indépendant dans `components/`.
2. **Assemblage HTML** : Les pages finales sont créées en fusionnant ces fragments.
3. **Zéro Redondance** : Les composants ne doivent pas inclure les balises `<head>` ou `<body>`, seulement le contenu HTML nécessaire.
4. **Style Standardisé** : Utilisation de Tailwind CSS et Lucide Icons, identique à la partie publique.

##  Sommaire des Spécifications
- [Dashboard Admin](prompts/dashboardAdmin.md )

