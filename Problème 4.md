# MATH 60231 — Devoir 1

## Problème 4 [15 points]: Combinaison de simulations et de valeur à risque

Dans ce problème, vous évaluerez comment les estimations historiques de la valeur à risque (VaR) évoluent dans le temps et comment ces changements pourraient être interprétés par un comité de risque financier. Vous travaillerez avec l’une des actions individuelles utilisées précédemment ou générerez de nouveaux rendements synthétiques en utilisant une distribution de Student-t à 3 degrés de liberté pour simuler une série avec des queues épaisses réalistes.

### a. Statistiques descriptives et analyse initiale [3 points]

1.  **Présentez les statistiques sommaires de base** (moyenne, écart-type, asymétrie, aplatissement) pour votre série de rendements choisie.
2.  **Incluez des graphiques** des séries chronologiques bien étiquetés des niveaux de rendement.
3.  Si vous utilisez des données simulées, **expliquez la structure du Processus Générateur de Données (PGD)**.
4.  **Commentez** si la distribution semble symétrique, à queues épaisses ou volatile dans le temps.
5.  **Établissez brièvement un lien** entre vos résultats et ce que nous pourrions attendre en pratique des rendements d’actifs réels.

### b. VaR historique avec fenêtre mobile [4 points]

1.  **Calculez une VaR historique à 5%** en utilisant une fenêtre mobile de 250 jours.
2.  **Tracez la série chronologique résultante** de la VaR estimée aux côtés des rendements réalisés.
3.  **Indiquez clairement où se produisent les violations** (c’est-à-dire où les rendements réels tombent en dessous de la VaR).
4.  **Interprétez le moment et le regroupement** de ces violations.
5.  Y a-t-il des périodes où le modèle semble **trop lent à réagir**?

### c. VaR historique avec fenêtre expansive [4 points]

1.  **Calculez maintenant la même VaR historique à 5%** en utilisant une fenêtre expansive (commençant avec 250 jours et augmentant d’une observation à chaque fois).
2.  **Tracez les estimations de VaR résultantes** et comparez leur stabilité et leur réactivité aux estimations de la fenêtre mobile.
3.  **Quelle méthode de fenêtrage est plus conservatrice?**
4.  **Laquelle est plus sensible aux chocs récents?**

### d. Interprétation pour un comité de risque [4 points]

Supposez qu’on vous demande d’expliquer une augmentation récente des estimations de VaR à un comité de risque, même si les rendements ont été en grande partie positifs dans le passé récent.

**Rédigez une brève explication** (environ 2 à 3 phrases) interprétant ce comportement en termes de :
*   Volatilité des rendements
*   Structure de fenêtre temporelle
*   Logique sous-jacente aux mesures de risque fondées sur les quantiles

Votre explication devrait refléter une compréhension claire de ce que le modèle capture et de la façon dont cela pourrait être communiqué à des intervenants non techniques.
