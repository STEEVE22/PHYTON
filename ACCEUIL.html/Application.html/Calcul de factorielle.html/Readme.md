<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exercices - Calcul de Factoriel</title>
    <link rel="stylesheet" href="style.css"> <!-- Lien vers le style -->
</head>
<body>

    <header>
        <h1>Exercices de Codage en Python - Calcul de Factoriel</h1>
        <p>Découvrez ci-dessous une série d'exercices pour apprendre et maîtriser le calcul du factoriel.</p>
    </header>

    <section>
        <h2>Exercice 1 : Calculer le Factoriel d'un Nombre (Boucle `for`)</h2>
        <pre><code>
# Calculer le factoriel d'un nombre donné
n = int(input("Entrez un nombre entier positif : "))
fact = 1
for i in range(1, n + 1):
    fact *= i
print(f"Le factoriel de {n} est {fact}")
        </code></pre>
    </section>

    <section>
        <h2>Exercice 2 : Calculer le Factoriel d'un Nombre (Boucle `while`)</h2>
        <pre><code>
# Calculer le factoriel d'un nombre donné
n = int(input("Entrez un nombre entier positif : "))
fact = 1
i = 1
while i <= n:
    fact *= i
    i += 1
print(f"Le factoriel de {n} est {fact}")
        </code></pre>
    </section>

    <section>
        <h2>Exercice 3 : Calculer le Factoriel avec une Fonction Récursive</h2>
        <pre><code>
# Définir une fonction récursive pour calculer le factoriel
def factoriel(n):
    if n == 0 or n == 1:
        return 1
    return n * factoriel(n - 1)

# Demander un nombre à l'utilisateur
n = int(input("Entrez un nombre entier positif : "))
print(f"Le factoriel de {n} est {factoriel(n)}")
        </code></pre>
    </section>

    <section>
        <h2>Exercice 4 : Calculer le Factoriel de 100</h2>
        <pre><code>
# Calculer le factoriel de 100
fact = 1
for i in range(1, 101):
    fact *= i

# Extraire les trois premiers chiffres
print(str(fact)[:3])
        </code></pre>
    </section>

    <section>
        <h2>Exercice 5 : Vérifier si un Nombre Est Factoriel</h2>
        <pre><code>
# Vérifier si un nombre est un factoriel
def est_factoriel(n):
    i = 1
    fact = 1
    while fact < n:
        i += 1
        fact *= i
    return fact == n

# Demander un nombre à l'utilisateur
n = int(input("Entrez un nombre entier : "))
if est_factoriel(n):
    print(f"{n} est un factoriel.")
else:
    print(f"{n} n'est pas un factoriel.")
        </code></pre>
    </section>

    <footer>
        <p>Pratiquez ces exercices pour maîtriser le calcul du factoriel et ses différentes applications en Python.</p>
    </footer>

</body>
</html
