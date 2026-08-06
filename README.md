# Grille
Grille de mots meles
from word_search_generator import WordSearch

# 1. Votre liste de mots présélectionnés
mots = ["LION", "CHAT", "CHIEN", "POULE", "SOURIS"]

# 2. Création de la grille (ex: 8x8 pour des enfants de 7-8 ans)
puzzle = WordSearch(mots, size=8)

# 3. Restriction des directions : Uniquement Est (horizontal) et Sud (vertical)
puzzle.directions = "E,S"

# 4. Affichage ou sauvegarde en PDF / TXT
puzzle.show()
puzzle.save(path="grille_enfants.pdf")
