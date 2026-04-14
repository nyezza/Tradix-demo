# Tradix by Yezza — Gestion pour courtiers en poisson

<div align="center">

![Logo Tradix](Logo.png)

**Digitaliser le commerce de poisson. Simple. Rapide. 100% hors ligne.**

[![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python)](https://python.org)
[![Flask](https://img.shields.io/badge/Flask-3.0-black?logo=flask)](https://flask.palletsprojects.com)
[![SQLite](https://img.shields.io/badge/SQLite-intégré-003B57?logo=sqlite)](https://sqlite.org)
[![Version](https://img.shields.io/badge/version-5.0-green)]()
[![License](https://img.shields.io/badge/licence-Propriétaire-red)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux-lightgrey)]()

[Vidéo démo](https://vimeo.com/1182304860?fl=pl&fe=sh) · [yezzatech.tn](https://www.yezzatech.tn)

> ⚠️ **Dépôt vitrine** — Le code source est propriétaire et non distribué.
> Pour toute demande de licence ou collaboration : [nadhir.y@yezzatech.tn](mailto:nadhir.y@yezzatech.tn)

> *"Plus de commerce, moins de calculs."*

</div>

---

## Contexte

Le commerce de poisson fonctionne encore majoritairement avec des cahiers papier et des calculs manuels. Tradix digitalise ce métier avec un outil **simple, adapté au terrain et 100% hors ligne**.

---

## Vidéo démo

[![Tradix Demo](https://vimeo.com/1182304860?fl=pl&fe=sh)

> Démonstration complète — tous les rôles testés en conditions réelles.

---

## Fonctionnalités

| Module | Description |
|--------|-------------|
| **Bons d'achat** | Multi-espèces · Numérotation automatique A2026-XXXXXX |
| **Bons de vente** | Multi-espèces · Stock temps réel · Numérotation V2026-XXXXXX |
| **Stock** | Calculé dynamiquement · 46 espèces FR+AR |
| **Caisses** | Traçabilité physique · Garanties · Retours |
| **Impayés** | Ancienneté en jours · Achats et ventes |
| **Avances** | Pêcheurs et clients |
| **Exports Excel** | 8 types de rapports |
| **Sauvegardes** | ZIP automatiques · Rétention 30 fichiers |
| **Audit** | Journal complet de toutes les actions |

---

## Architecture

```
Flask 3.0 (Waitress WSGI)
    ↕ SQLite (intégré)
Jinja2 Templates (HTML/CSS/JS)
```

**Points techniques notables :**
- Schéma SQLite v5.0 : **22 tables · 15 vues SQL · 12 triggers**
- RBAC 3 niveaux avec décorateurs `@niveau_min(n)`
- Annulation obligatoire avec motif (jamais de suppression physique)
- Sauvegarde ZIP automatique à chaque démarrage
- Distribution Windows via PyInstaller (exécutable .exe)
- 100% hors ligne — aucune donnée ne quitte le poste

---

## Rôles

| Rôle | Niveau | Accès |
|------|--------|-------|
| **Admin** | 3 | Complet + gestion utilisateurs |
| **Gérant** | 2 | Opérationnel + paramètres + audit |
| **Courtier** | 1 | Saisie et consultation |

---

## Licence & Contact

Ce logiciel est la propriété exclusive de **Yezza Tech**.
Le code source n'est pas distribué publiquement.

- 📧 [nadhir.y@yezzatech.tn](mailto:nadhir.y@yezzatech.tn)
- 🌐 [yezzatech.tn](https://www.yezzatech.tn)
- 💼 [linkedin.com/in/nyezza](https://linkedin.com/in/nyezza)

---

## Autres projets Yezza Tech

| Projet | Description | Lien |
|--------|-------------|------|
| **Voltix** | ERP complet pour PME | [github.com/nyezza/voltix](https://github.com/nyezza/voltix) |
| **Medix** | SaaS de gestion de cabinet médical | [github.com/nyezza/medix](https://github.com/nyezza/medix) |

---

<div align="center">

Développé par **[Nadhir Yezza](https://www.yezzatech.tn)** · Yezza Tech · Tunisie

**Version 5.0** · Avril 2026

</div>
