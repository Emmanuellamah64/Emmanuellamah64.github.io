# CLAUDE.md — Portfolio Emmanuel LAMAH
# Instructions complètes pour Claude Code

## Contexte du projet

Tu dois générer un portfolio professionnel pour **Emmanuel LAMAH**, Ingénieur DevSecOps & AI Security Engineer.
Ce portfolio est destiné aux recruteurs tech à Paris.
Il sera hébergé sur GitHub Pages à l'adresse : `https://emmanuellamah64.github.io`

---

## Structure du projet à générer

```
portfolio/
├── index.html          # Page principale (tout en un fichier)
├── CLAUDE.md           # Ce fichier
└── README.md           # Instructions de déploiement
```

Le portfolio est un **fichier HTML unique** avec CSS et JS intégrés.
Pas de framework, pas de build tool, pas de dépendances — déployable directement sur GitHub Pages.

---

## Identité visuelle

### Palette de couleurs
```css
--bg:           #080d1a   /* Fond principal — bleu nuit profond */
--surface:      #0f1629   /* Cartes et panels */
--surface2:     #151e35   /* Surfaces secondaires */
--gold:         #C9A84C   /* Accent principal — or Versailles */
--gold-light:   #E2C068   /* Or au hover */
--green:        #1D9E75   /* Statut actif / running */
--green-dim:    rgba(29,158,117,0.15)
--text:         #EEF0F5   /* Texte principal */
--text-dim:     #7A8499   /* Texte secondaire */
--text-muted:   #3D4A66   /* Texte très atténué */
--border:       rgba(255,255,255,0.06)
--border-gold:  rgba(201,168,76,0.25)
```

### Typographie
```css
--mono: 'JetBrains Mono', monospace   /* Labels, tags, code, nav logo */
--sans: 'Inter', system-ui, sans-serif /* Corps et titres */
```

Importer depuis Google Fonts :
```html
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
```

### Signature visuelle
- **Élément distinctif** : un panneau "System Status" façon terminal de production, montrant CGS et EPICO-IA comme systèmes en cours d'exécution avec un point clignotant vert
- **Accent or** : rappel subtil du Château de Versailles sans être ostentatoire
- **Fond bleu nuit** : sérieux, technique, professionnel

---

## Informations personnelles

```
Nom          : Emmanuel LAMAH
Titre        : Ingénieur DevSecOps & AI Security Engineer
Localisation : Cergy (95), France — Paris region
Email        : lamahemmanuel64@gmail.com
Téléphone    : +33 7 59 41 48 28
LinkedIn     : linkedin.com/in/emmanuel-lamah
GitHub       : github.com/Emmanuellamah64
Disponibilité: CDI dès janvier 2027 — Paris
```

---

## Contenu de chaque section

### Section 1 — HERO

**Statut badge** (JetBrains Mono, vert avec dot clignotant) :
```
● Available for CDI — Paris · Jan 2027
```

**Nom** (grande taille, accent or sur "LAMAH") :
```
Emmanuel
LAMAH
```

**Sous-titre** :
```
AI Security Engineer & DevSecOps — Château de Versailles
```

**Description** :
```
I build secure AI systems in production. Sole developer of two platforms
at the Palace of Versailles — from climate sensor infrastructure to a
sovereign multi-agent LLM architecture.

MSc Cybersecurity (CY Tech, highest honors) · MSc AI/Big Data (IPSSI) · CompTIA Security+
```

**Boutons CTA** :
- `Contact me` → mailto:lamahemmanuel64@gmail.com (bouton or plein)
- `LinkedIn` → https://linkedin.com/in/emmanuel-lamah (bouton contour)
- `GitHub` → https://github.com/Emmanuellamah64 (bouton contour)

**Panel System Status** (après les boutons) :
```
┌─ ● ● ●  PRODUCTION SYSTEMS — EPV INFRASTRUCTURE ─────────────────┐
│ ● RUNNING  CGS v1.0      Climate Graphing Software · Django/React  │
│ ● RUNNING  EPICO-IA v2.0 Multi-agent SaaS · LangGraph · RAG       │
└───────────────────────────────────────────────────────────────────┘
```
- Points verts avec animation `pulse` (opacity 1 → 0.3 → 1, 2.5s)
- Fond `--surface`, bordure `--border`, police `JetBrains Mono` 12px
- Tags "RUNNING" en vert sur fond `rgba(29,158,117,0.15)`

---

### Section 2 — PROJECTS

**Label** : `Featured Work` (mono, or, uppercase)
**Titre** : `Production Platforms`
**Sous-titre** : `Built solo at the Château de Versailles — real systems, real constraints, real users.`

**Grille 2 colonnes** (1 colonne sur mobile)

#### Projet 1 — EPICO-IA
```
Année      : 2026 · Alternance
Nom        : EPICO-IA
Rôle       : // Sole Developer · SaaS · Production
Description:
  Multi-tenant SaaS open to any museum worldwide. Integrates a 4-agent
  AI system (LangGraph), real-time anomaly detection (Isolation Forest),
  72h forecasting (Prophet/Meta), and a sovereign on-premise Mistral LLM
  with RAG over Qdrant. Full DevSecOps pipeline — OWASP, SAST/DAST,
  RGPD/AI Act compliant.

Stack tags : FastAPI · React TS · LangGraph · Mistral · Qdrant ·
             TimescaleDB · Docker · GitHub Actions
```

#### Projet 2 — CGS
```
Année      : 2025 · Stage MSc
Nom        : CGS
Rôle       : // Sole Developer · Full-Stack · Production
Description:
  Climate Graphing Software — full-stack platform collecting real-time
  data from climate sensors across the Château de Versailles. Built to
  OWASP Top 10 standards, with JWT auth, role management, and a MongoDB
  time-series backend. Feeds EPICO-IA with historical data.

Stack tags : Django · React · MongoDB · Python · OWASP · JWT · REST API
```

**Style des cartes** :
- Fond `--surface`, bordure `--border`
- Ligne or en haut : `linear-gradient(90deg, var(--gold), transparent)` height 2px
- Au hover : border-color `--border-gold`, translateY(-2px)
- Nom du projet en `--gold`
- Rôle en `--green`, police mono
- Tags en fond `--surface2`, police mono 10px

---

### Section 3 — SKILLS

**Label** : `Expertise`
**Titre** : `Technical Stack`
**Sous-titre** : `Core competencies across AI, security, and infrastructure.`

**Grille** : `repeat(auto-fit, minmax(200px, 1fr))`

#### Groupes de compétences

| Groupe | Compétences |
|--------|-------------|
| AI & GenAI | LangGraph · RAG · Qdrant · Mistral · Ollama · Isolation Forest · Prophet · MLOps |
| DevSecOps | OWASP Top 10 · SAST/DAST · Snyk · SonarQube · Trivy · RGPD · AI Act |
| Backend | FastAPI · Django · Python · REST API · Celery · Redis · TimescaleDB · MongoDB |
| Infrastructure | Docker · Kubernetes · GitHub Actions · Terraform · Ansible · AWS · Linux |
| Network Security | Wireshark · Nmap · Burp Suite · LDAP · Active Directory · VLAN · ACL · RHEL |
| Frontend | React TypeScript · JavaScript · HTML/CSS |

#### Certifications (sous la grille)

```
🛡️ CompTIA Security+ 701          — CompTIA
🔐 Jr Penetration Tester           — TryHackMe
🎓 MSc Cybersecurity — Mention TB  — CY Tech / RNCP Niv. 7
```

---

### Section 4 — EXPERIENCE

**Label** : `Background`
**Titre** : `Experience`
**Sous-titre** : `Progressive track from network security to production AI systems.`

**Layout** : grille `140px 1fr`, séparation par bordure bottom

#### Expériences dans l'ordre

```
Mar 2026 – Jan 2027
Assistant R&D DevSecOps IA / Big Data
Château de Versailles — Alternance
→ Designed and built EPICO-IA from scratch — a multi-tenant SaaS integrating
  sovereign AI (LangGraph, RAG, Mistral on-premise), anomaly detection, and
  full DevSecOps pipelines.
Tags: FastAPI · LangGraph · Qdrant · Docker · OWASP · SAST/DAST

Jul 2025 – Dec 2025
Assistant R&D DevSecOps
Château de Versailles — Stage
→ Built CGS, a full-stack Django/React platform for real-time climate sensor
  data collection, secured to OWASP Top 10 standards with JWT auth and audit trail.
Tags: Django · React · MongoDB · OWASP

Jun 2023 – Nov 2024
Network, Systems & Security Engineer
Direction Générale des Douanes de Guinée
→ Hardening of critical infrastructure under RHEL, LDAP identity management,
  firewall and VLAN configuration, internal app development with Spring Boot/Java.
Tags: RHEL · LDAP · Spring Boot · Cisco

Jan 2024 – Jun 2024
DevOps Engineer
EliteTech Consulting — Tunis
→ Built CI/CD pipelines, containerized applications with Docker, orchestrated
  services with Kubernetes, automated infrastructure on AWS.
Tags: Docker · Kubernetes · AWS · Terraform
```

---

### Section 5 — CONTACT

**Centré**, max-width 560px, carte avec bordure `--border-gold`

```
Titre : Let's work together

Texte : Looking for a CDI in Paris from early 2027.
        Open to DevSecOps, AI Security, GenAI, MLOps roles.

Liens :
  ✉  lamahemmanuel64@gmail.com  → mailto:...
  in LinkedIn                   → https://linkedin.com/in/emmanuel-lamah
  ⌥  GitHub                     → https://github.com/Emmanuellamah64
```

---

## Navigation fixe

```
Logo (mono) : EL // Portfolio
Liens       : Projects · Skills · Experience · Contact
```

- Position fixed, hauteur 60px
- Fond `rgba(8,13,26,0.92)` + `backdrop-filter: blur(12px)`
- Bordure bottom `--border`
- Scroll smooth via `html { scroll-behavior: smooth; }`

---

## Animations

```css
/* Point clignotant */
@keyframes pulse {
  0%, 100% { opacity: 1; }
  50%       { opacity: 0.3; }
}

/* Appliquer sur les dots verts */
.dot-live, .sys-running {
  animation: pulse 2s ease-in-out infinite;
}
```

Pas d'autres animations — sobriété voulue.

---

## Responsive

```css
@media (max-width: 680px) {
  .project-grid { grid-template-columns: 1fr; }
}

@media (max-width: 600px) {
  nav { padding: 0 20px; }
  section { padding: 60px 20px; }
  .exp-item { grid-template-columns: 1fr; gap: 4px; }
  .contact-card { padding: 32px 20px; }
}
```

---

## Footer

```
Font : JetBrains Mono 11px, couleur --text-muted
Texte : Built by Emmanuel LAMAH · Paris, France · 2026
```

---

## README.md à générer

```markdown
# Portfolio — Emmanuel LAMAH

Portfolio professionnel hébergé sur GitHub Pages.

## Déploiement

1. Ce repository doit être nommé `Emmanuellamah64.github.io`
2. Renommer `index.html` si nécessaire
3. Settings → Pages → Deploy from branch → main
4. URL : https://emmanuellamah64.github.io

## Stack

HTML · CSS · JavaScript vanilla — aucune dépendance externe sauf Google Fonts.
```

---

## Instructions pour Claude Code

1. Génère `index.html` en un seul fichier avec CSS et JS intégrés dans `<style>` et `<script>`
2. N'utilise aucun framework JS (pas de React, Vue, etc.)
3. N'utilise aucun CDN sauf Google Fonts
4. Respecte exactement la palette de couleurs définie
5. Respecte exactement le contenu de chaque section
6. Le fichier doit être fonctionnel en ouvrant directement dans un navigateur (file://)
7. Génère aussi `README.md` avec les instructions de déploiement GitHub Pages
8. Vérifie que tous les liens href sont corrects
9. Assure-toi que la navigation anchor fonctionne (id="projects", id="skills", etc.)
10. Le résultat final doit être prêt à pusher sur GitHub sans modification
