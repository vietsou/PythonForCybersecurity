
## 1. Variables et Types de Données

### Déclaration et Initialisation

```python
# Déclarer une variable
mon_nom = "Jean Dupont"

# Afficher la valeur
print(mon_nom)
```

### Types de données

```python
chaine: str = "Chaîne de caractères"
entier: int = 123
flottant: float = 1.23
booleen: bool = True / False
```

---

## 2. Structures de Données

### Listes

#### Création

```python
# Liste de périphériques réseau
reseau = ["Cisco", "Fortinet", "Linksys"]
```

#### Ajouter des éléments

```python
# Ajouter un élément à la fin
reseau.append("Netgear")

# Ajouter un élément à une position spécifique
reseau.insert(1, "Ubiquiti")

# Ajouter plusieurs éléments (sous forme de liste)
autres_reseaux = ["TP-Link", "Juniper"]
reseau.extend(autres_reseaux)
```

#### Accéder et Modifier

```python
# Accéder à un élément
print(reseau[0])  # Premier élément
print(reseau[-1])  # Dernier élément

# Slicing
print(reseau[1:3])  # Sous-liste des éléments 1 à 2
```

#### Supprimer des éléments

```python
# Supprimer par nom
reseau.remove("Cisco")

# Supprimer par index
del reseau[0]

# Vider la liste
reseau.clear()
```

#### Trier et Inverser

```python
reseau.sort()  # Trier par ordre alphabétique
reseau.reverse()  # Inverser l'ordre
```

#### Comptage et Recherche

```python
print(reseau.count("Fortinet"))  # Nombre d’occurrences
print(reseau.index("Linksys"))  # Index de "Linksys"
```

### Tuples

```python
# Création d’un tuple
equipements = ("Switch", "Routeur")

# Accéder aux éléments
print(equipements[0])
```

---

## 3. Boucles

### Boucle `for`

```python
# Parcourir une liste
for appareil in reseau:
    print(appareil)
```

### Boucle `while`

```python
i = 0
while i < len(reseau):
    print(reseau[i])
    i += 1
```

### Utilisation de `range`

```python
# Générer une séquence de nombres
for i in range(5):
    print(i)  # Affiche 0 à 4
```

---

## 4. Fonctions

### Définir une fonction

```python
def afficher_nom(nom):
    print(f"Bonjour, {nom}!")

afficher_nom("Alice")
```

### Retourner une valeur

```python
def addition(a, b):
    return a + b

print(addition(2, 3))  # Affiche 5
```

---

## 5. Gestion des Fichiers

### Lire un fichier

```python
with open("fichier.txt", "r") as fichier:
    contenu = fichier.read()
    print(contenu)
```

### Écrire dans un fichier

```python
with open("fichier.txt", "w") as fichier:
    fichier.write("Nouveau contenu")
```

---

## 6. Modules

### Importer un module

```python
import math
print(math.sqrt(16))  # Affiche 4
```

### Modules externes

```bash
# Installer un module avec pip
pip install requests
```

```python
import requests
response = requests.get("https://example.com")
print(response.status_code)
```

