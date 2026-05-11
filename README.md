# 🔐 Analyse de Vulnérabilités - Nessus

Ce projet consiste en une analyse de vulnérabilités réalisée dans un cadre académique à l’aide de l’outil Nessus.  
L’objectif est d’identifier des failles de sécurité, de construire une chaîne de vulnérabilités et d’évaluer leur impact à l’aide du score CVSS.

---

## 🎯 Objectifs du projet

- Détection de vulnérabilités sur des machines via Nessus
- Sélection et analyse de vulnérabilités critiques
- Construction d’une chaîne d’exploitation
- Évaluation du risque via CVSS
- Proposition de solutions de remédiation
- Recommandations de sécurité

---

## 🛠️ Outils utilisés

- Nessus (scan de vulnérabilités)
- National Vulnerability Database (NVD)
- CVSS v3.1 (évaluation des risques)

---

## 🔎 Vulnérabilités étudiées

### CVE-2016-2118 (Samba Badlock)
- Type : Man-in-the-Middle (MITM)
- Impact : Confidentialité, intégrité et disponibilité élevées
- Score CVSS : 7.5

### CVE-2016-2183 (SWEET32)
- Type : Faiblesse cryptographique (3DES)
- Impact : Confidentialité élevé
- Score CVSS : 7.5

---

## 🔗 Chaîne de vulnérabilités

Une chaîne d’attaque a été construite :

1. Exploitation de Samba Badlock (accès initial / interception)
2. Exploitation de SWEET32 (décryptage de données)
3. Compromission de la confidentialité des échanges

### ⚠️ Score final de la chaîne :
**CVSS : 9.72 (Critique)**

---

## 🛡️ Mesures de sécurité

### Correction de Samba Badlock
- Mise à jour de Samba
- Désactivation SMBv1
- Activation SMB signing
- Restriction des ports SMB (139/445)

### Correction de SWEET32
- Désactivation de 3DES
- Utilisation de TLS 1.2 / TLS 1.3
- Migration vers AES / ChaCha20

---

## 📊 Résultat

Le projet montre qu’une chaîne de vulnérabilités peut augmenter fortement le niveau de risque global, même si chaque faille individuellement semble modérée.

---

## 👨‍💻 Auteurs

- Mamadou Talibe DIALLO  
- Abdoulaye LOUBARASSEM  

Projet académique – Cybersécurité défensive
