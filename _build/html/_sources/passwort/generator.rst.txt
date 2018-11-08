Passwort-Generator
==================

Das Programm wählt die vier Teile des Passworts zufällig aus, setzt sie zusammen und zeigt das Passwort an. Wenn du das Passwort nicht magst, wiederholt es die Schritte, gefällt es dir, endet das Programm.

.. code-block:: python

   import string
   import random

   die_adjektive = ['müde', 'blöd', 'furzend', 'stinkend', 'hungrig', 'schläfrig', 'flauschig', 'wuschelig', 'stachelig', 'pieksig', 'blau', 'rot', 'grün']
   die_nomen = ['Baum', 'Blatt', 'Stift', 'Wecker', 'Kaffee', 'Toaster', 'Pizza', 'Panda', 'Dinosaurier', 'Schlange', 'Anaconda', 'Mixer', 'Tumbler', 'Tisch']

   #  die Variablen 'adjektiv' und 'nomen' enthalten ein zufällig gewähltes Element aus der Liste
   adjektiv = random.choice(die_adjektive)
   nomen = random.choice(die_nomen)

   zahl = random.randrange(0,99)
   #sonderzeichen = random.string.punctuation()

   passwort = adjektiv + nomen + str(zahl)
   print("Das neue Passwort ist: %s" % passwort)

Beispiele
---------

 * wuscheligPizza89!
 * blauDinosaurier85#
 * schläfrigSchlange22-
 * wuscheligToaster82?



