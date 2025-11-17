## **Critères d’évaluation Coding Weeks**

### 1. **Documentation & Langue**

* **README complet et en anglais** :

  * Introduction au projet, contexte, but.
  * Instructions de lancement et d’installation.
  * Exemple minimal d’utilisation.
* **Commentaires et docstrings en anglais** :

  * Chaque fonction importante contient une docstring (conforme au style NumPy ou Google).
  * Pas de commentaire en français dans le code, TOUT doit être en anglais.
* **Documentation technique (bonus)** :

  * Diagramme, architecture ou workflow expliqué dans les `docs/`.

---

### 2. **Organisation et structure du projet**

* Arborescence claire et propre :

  * `.gitignore` bien rempli (enlève les fichiers de cache, datasets locaux, environnements virtuels…).
  * Code source dans un répertoire `src/` ou au nom du projet.
  * Fichiers de données éventuellement ignorés ou allégés.

* **Noms de fichiers conformes** :

  * Pas d’accents, d’espaces ou de caractères spéciaux dans les noms de fichiers ou de dossiers.

* Présence d’un fichier `requirements.txt`, `pyproject.toml` ou `environment.yml` pour installer facilement les dépendances.

---

### 3. **Qualité du code**

* **Respect des normes PEP8 avec formatage automatique**
  Le code Python doit respecter les conventions **PEP8**, qui définissent les bonnes pratiques en termes de nommage, indentation, longueur des lignes, espaces, etc.

Comment faire ? Installer le module *black* :

```bash
pip install black
```

Puis formater tout le projet sur la racine :

```bash
black .
```

* **Pas de duplication inutile, ni de code mort**.
* **Architecture modulaire** :

  * Pas de monofichier de 1000 lignes.
  * Utilisation de classes, fonctions, modules logiques.

---

### 4. **Tests & Validation**

* Présence d’un répertoire `tests/`.
* Utilisation de `pytest`
* Tests pour :

  * les fonctions principales,
  * les cas limites (edge cases).

---

### 5. **Gestion de version & collaboration**

* **Commits réguliers et descriptifs**, en anglais (ex. : `feat: add API to process images`).
* **Utilisation de branches** pour fonctionnalité ou refactoring (pas tout sur `main`).
* Pas de `merge` hasardeux (pas de "merge conflict" visible dans un fichier sélectionné).
