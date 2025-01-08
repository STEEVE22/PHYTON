<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exercices - Résolution des Équations Quadratiques</title>
    <link rel="stylesheet" href="style.css"> <!-- Lien vers le style -->
</head>
<body>

    <header>
        <h1>Exercices de Codage en Python - Résolution des Équations Quadratiques</h1>
        <p>Pratiquez la programmation Python avec ces exercices sur les équations quadratiques.</p>
    </header>

    <section>
        <h2>Exercice 1 : Résolution d'une Équation Quadratique (Formule Quadratique)</h2>
        <pre><code>
# Résolution d'une équation quadratique : ax² + bx + c = 0
import math

# Entrer les coefficients
a = float(input("Entrez le coefficient a : "))
b = float(input("Entrez le coefficient b : "))
c = float(input("Entrez le coefficient c : "))

# Calcul du discriminant
discriminant = b**2 - 4*a*c

if discriminant > 0:
    x1 = (-b + math.sqrt(discriminant)) / (2 * a)
    x2 = (-b - math.sqrt(discriminant)) / (2 * a)
    print(f"Les solutions sont x1 = {x1} et x2 = {x2}")
elif discriminant == 0:
    x = -b / (2 * a)
    print(f"La solution unique est x = {x}")
else:
    print("Pas de solution réelle.")
        </code></pre>
    </section>

    <section>
        <h2>Exercice 2 : Vérifier si une Équation Quadratique a des Solutions Réelles</h2>
        <pre><code>
# Vérifier si une équation quadratique a des solutions réelles
a = float(input("Entrez le coefficient a : "))
b = float(input("Entrez le coefficient b : "))
c = float(input("Entrez le coefficient c : "))

# Calcul du discriminant
discriminant = b**2 - 4*a*c

if discriminant >= 0:
    print("L'équation a des solutions réelles.")
else:
    print("L'équation n'a pas de solutions réelles.")
        </code></pre>
    </section>

    <section>
        <h2>Exercice 3 : Afficher les Racines Complexes si le Discriminant est Négatif</h2>
        <pre><code>
# Résolution d'une équation quadratique avec racines complexes
import cmath

a = float(input("Entrez le coefficient a : "))
b = float(input("Entrez le coefficient b : "))
c = float(input("Entrez le coefficient c : "))

# Calcul des racines même si le discriminant est négatif
discriminant = b**2 - 4*a*c
x1 = (-b + cmath.sqrt(discriminant)) / (2 * a)
x2 = (-b - cmath.sqrt(discriminant)) / (2 * a)

print(f"Les solutions sont x1 = {x1} et x2 = {x2}")
        </code></pre>
    </section>

    <section>
        <h2>Exercice 4 : Résoudre une Équation Quadratique en Vérifiant les Cas de Coefficients Particuliers</h2>
        <pre><code>
# Gérer les cas particuliers d'une équation quadratique
a = float(input("Entrez le coefficient a : "))
b = float(input("Entrez le coefficient b : "))
c = float(input("Entrez le coefficient c : "))

if a == 0 and b == 0:
    print("Ceci n'est pas une équation valide.")
elif a == 0:
    x = -c / b
    print(f"Ceci est une équation linéaire. La solution est x = {x}")
else:
    discriminant = b**2 - 4*a*c
    if discriminant > 0:
        x1 = (-b + math.sqrt(discriminant)) / (2 * a)
        x2 = (-b - math.sqrt(discriminant)) / (2 * a)
        print(f"Les solutions sont x1 = {x1} et x2 = {x2}")
    elif discriminant == 0:
        x = -b / (2 * a)
        print(f"La solution unique est x = {x}")
    else:
        print("Pas de solution réelle.")
        </code></pre>
    </section>

    <footer>
        <p>Continuez à vous entraîner avec ces exercices pour comprendre les équations quadratiques et leur résolution en Python.</p>
    </footer>

</body>
</html>
