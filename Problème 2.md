# MATH 60231 — Devoir 1

---

MATH 60231 : Devoir#1
Professeur Anthony Sanford
Date limite : 2 novembre 2025 à 23 h 55 sur ZoneCours
Instructions :Pour ce travail, vous devez travailler en groupes detrois. Je ne m’occuperaipasde la créa-
tion des groupes. Il est de votre responsabilité de trouver des membres d’équipe pour votre devoir. Si vous
avez des difficultés à trouver une équipe, vous pouvez me contacter par courriel et j’essaierai de vous mettre
en contact avec d’autres personnes de la classe. Ce devoir comprenddeuxéléments à soumettre : 1) votre
rédaction et 2) votre code. Le fait de ne pas soumettre l’un de ces deux éléments sera considéré comme une
soumission incomplète. Votre code doit être écrit en Python. Votre code doit fonctionner de manière fluide
et être clairement annoté. Si vous avez utilisé des ressources en dehors de ce qui est assigné pour ce cours,
vousdevezdonner le crédit de la source. Par exemple, si vous avez recherché du code sur Google et utilisé
ce que vous avez trouvé, indiquez la source. Sinon, vous trichez. Votre rédaction a comme objectif d’analyser,
de discuter et d’interpréter vos résultats. Soumettre simplement un tableau sans en discuter clairement ne
constitue pas une réponse à la question. Considérez ce que je fais en classe - je présente un thème et j’en
discute. Pensez à votre rédaction de la même manière. Vous interprétez vos résultats pour quelqu’un qui lit
votre rapport. Veuillez noter que les règles de HEC Montréal concernant le plagiat s’appliquent à la fois à
vos réponses écrites et à votre code informatique.
Il y a 4 questions en plusieurs parties, les points pour chaque question/partie sont indiqués ci-dessous. Pour
chaque partie, il y a quatre notes possibles :
— E : C’est la note si vous n’écrivez littéralement rien. Ça vaut 0 %.
— C : C’est la note si vous ne comprenez vraiment pas ce que vous faites... mais que vous avez écrit
quelque chose. Ça vaut 50%.
— B : C’est la note si vous avez obtenu la réponse en grande partie correcte. Ça vaut 80%. Ce sera
probablement la note la plus courante.
— A : C’est la note si votre réponse est aussi bonne (ou meilleure!) que la mienne. Ça vaut 100%.
Remarque: les commentaires dans votre code qui me permettent de comprendre facilement ce que vous
avez essayé de faire peuvent améliorer votre note. Un code python particulièrement laid ou inélégant peut
réduire votre note de 10% (par exemple, si vous faites beaucoup de copier-coller parce que vous ne savez pas
comment utiliser efficacement les boucles, les fonctions ou les opérations de tableau). Vous pouvez également
perdre des points si votre code ne s’exécute pas correctement ou ne fournit pas la même solution que votre
réponse écrite.
1

Problème 1 [10 points]
Cette question évalue votre capacité à suivre les consignes. Si vous respectez les instructions de ce devoir,
vous obtiendrez la note maximale pour cette question.
a.Indiquez les noms des membres de votre équipe [2 points]
b.Dactylographiez vos réponses (c’est-à-dire que vous n’avez pas remis votre devoir écrit à la main) [2
points]
c.Présentez votre devoir sous forme de rapport rédigé, et non simplement du code que vous soumettez
(incluant une mise en forme et un étiquetage appropriés des tableaux et des graphiques) [2 points]
d.Fournissez le code Python à l’appui de vos réponses [2 points]
e.Votre code Python fonctionne effectivement de façon autonome et produit les réponses que vous avez
soumises dans votre rapport [2 points]
Problème 2 [40 points], Mesure du risque
Pour cette question, vous devrez recueillir des données pour quatre titres : un indice représentatif du
marché américain, une action du secteur financier, une action du secteur technologique et une action du
secteur énergétique. Pour chaque titre, obtenez des données quotidiennes de prix ou de niveau du 3 janvier
2012 au 3 janvier 2023. Chaque étudiant de votre équipe doit sélectionner une action par secteur en utilisant
la première lettre de son prénom. Par conséquent, votre équipe disposera de trois actions distinctes pour
chacun des trois secteurs. S’il n’existe aucune action actuellement négociée dans un secteur commençant
par la lettre qui vous est attribuée, utilisez la lettre suivante de votre nom de famille. Vous ne pouvez pas
sélectionner des sociétés disparues ou radiées de la cote. Utilisez uniquement des actions qui ont été cotées
en bourse pendant toute la période d’échantillonnage.
a.Pour chaque titre, calculez les rendements, fournissez des statistiques descriptives et présentez des
graphiques de séries chronologiques pour vos données. Assurez-vous d’étiqueter correctement vos gra-
phiques et de discuter des résultats (tant les statistiques descriptives que les graphiques). [5 points]
Pour les questions suivantes, concentrez-vous exclusivement sur l’indice de marché et sur les secteurs tech-
nologique et énergétique.
b.Estimez la valeur à risque (VaR) historique à 1% et à 5% ainsi que le déficit attendu (ES) pour l’indice
de marché, l’action technologique et l’action énergétique. Utilisez des quantiles empiriques (c’est-à-dire
des méthodes non paramétriques fondées directement sur la distribution historique des rendements).
Commenteztoutedifférencenotabledanslerisquedequeueentrelessecteursetinterprétezlesrésultats
à la lumière du profil de risque généralement associé à chaque secteur. [5 points]
c.Supposez maintenant que les rendements sont i.i.d. et distribués normalement, comme c’est souvent le
cas en pratique. Calculez la VaR paramétrique (gaussienne) et l’ES aux mêmes niveaux de confiance.
Comparezcesrésultatsàceuxquevousavezobtenusàlapartie(b).Discutezsil’hypothèsedenormalité
conduit à une sous-estimation ou à une surestimation du risque dans ces cas. Pourquoi cette approche
pourrait-elle induire en erreur un gestionnaire de risques? [5 points]
2

d.Supposez que votre gestionnaire de risques souhaite une estimation de la VaR qui s’adapte aux condi-
tions changeantes du marché. Une approche simple consiste à permettre à la volatilité d’évoluer dans
le temps en fonction de l’historique récent des rendements — même sans formuler d’hypothèses pa-
ramétriques fortes. Utilisez une règle récursive (fondée sur la volatilité passée pondérée) pour estimer
une VaR à un jour d’avance variant dans le temps pour chaque série. Tracez la série chronologique de
VaR résultante et comparez-la aux rendements réalisés. Discutez des moments où le modèle signale un
risque élevé et si ces signaux semblent raisonnables. [5 points]
e.Les tests de résistance constituent un élément clé de la gestion moderne des risques. Pour explorer
comment vos modèles se comportent pendant les crises, insérez artificiellement une courte séquence
de rendements négatifs importants dans vos données (par exemple, une panique boursière simulée).
Réestimez les trois modèles de VaR — historique, gaussien et récursif — et comparez la rapidité avec
laquelle chaque modèle s’adapte. Lequel absorbe le choc le plus rapidement? Lequel est trop lent à
s’ajuster? Quelles sont les conséquences potentielles d’un ajustement retardé dans des contextes réels?
[5 points]
f.On s’attend à ce que les modèles de risque prédisent correctement la fréquence des pertes extrêmes.
Utilisez la statistique de test de couverture définie ci-dessous pour évaluer si chaque modèle présente
le taux de violation empirique correct. Rapportez vos résultats et interprétez-les. Que signifie pour un
modèle d’avoir trop peu ou trop de violations? [7,5 points]
S=(#violations−αT)√
α(1−α)T
g.En plus de correspondre au taux de violation global, les bons modèles de risque devraient produire des
violations qui ne sont pas regroupées. Si les violations tendent à se produire en séquences consécutives,
le modèle pourrait manquer des dynamiques sous-jacentes ou une dépendance temporelle. Utilisez
un test de séquences fondé sur le nombre attendu de transitions entre les états de violation et de
non-violation. Interprétez vos résultats dans le contexte du comportement financier — par exemple,
comment le regroupement de violations pourrait-il influencer les réponses des gestionnaires de fonds
face au risque? [7,5 points]
Problème 3 [35 points], Simulations
Cette question explore le comportement de modèles de risque courants lorsque le processus générateur
de données (PGD) s’écarte des hypothèses standard. Vous simulerez des rendements sous différents PGD et
évaluerez la performance de divers modèles de VaR. Cela vous permet de tester la robustesse des modèles
et de réfléchir à la façon dont les violations réelles des hypothèses distributionnelles pourraient fausser les
estimations du risque.
a.Simulezdeuxsériesderendementsdelongueurégale:l’unetiréed’unedistributiongaussiennestandard
etl’autred’unedistributionàqueuesépaissestellequeladistributiondeStudent-tà3degrésdeliberté.
Normalisez les deux séries pour qu’elles aient la même variance inconditionnelle. Pour chaque série de
rendements simulée, calculez et rapportez les statistiques sommaires de base (moyenne, écart-type,
asymétrie, aplatissement) et représentez la distribution à l’aide d’un histogramme ou d’une estimation
par noyau de densité. Discutez et interprétez tout écart par rapport à la normalité, particulièrement
dans les queues. [5 points]
3

b.Estimez la VaR à 5% et le déficit attendu pour les deux séries simulées en utilisant trois méthodes : (i)
le quantile empirique, (ii) une approche paramétrique gaussienne, et (iii) une approche fondée sur la
distributiont(avec des degrés de liberté connus). Comparez les résultats et commentez la sensibilité
de chaque méthode à la forme distributionnelle des rendements. Quelles sont les implications pratiques
pour la gestion des risques lorsqu’on utilise la mauvaise distribution? [6 points]
c.Utilisez le rééchantillonnage bootstrap pour générer une distribution pour la VaR empirique à 5% à
partir des données simulées de Student-t. Tracez la distribution bootstrap et rapportez un intervalle de
confiance à 95% pour l’estimation de la VaR. Quelle est la largeur de cet intervalle, et que suggère-t-elle
quant à la précision et à la fiabilité de la VaR historique dans de petits échantillons? [6 points]
d.Simulez maintenant une série de rendements qui imite un environnement de marché avec des krachs
rares mais graves. La plupart du temps, les rendements devraient sembler normaux, mais occasionnel-
lement, ils devraient présenter de grands chocs négatifs. Plus précisément, simulez des rendements de
sorte que chaque observation soit tirée d’une distribution normale de moyenne nulle et d’écart-type de
1% avec une probabilité de 95%, et d’une distribution normale de moyenne−10% et d’écart-type de
4% avec une probabilité de 5%. Cette règle simple crée une série de rendements avec une asymétrie et
des queues épaisses réalistes, sans nécessiter de connaissances formelles des modèles à changements de
régime. En utilisant ces données simulées, estimez la valeur à risque à 5% en utilisant trois méthodes :
(1) le quantile empirique (c’est-à-dire la VaR historique), (2) la VaR paramétrique gaussienne fondée
sur la moyenne et l’écart-type de l’échantillon, et (3) la méthode récursive fondée sur la volatilité du
problème 2. Comparez les résultats et discutez quel modèle produit une estimation plus réaliste du
risque de baisse en présence de pertes rares mais extrêmes. Quel modèle est le plus robuste dans cet
environnement? Lequel peut sous-réagir ou sur-réagir? Expliquez comment ces différences pourraient
affecter les décisions financières en pratique. [8 points]
e.En utilisant une simulation bootstrap, évaluez la fiabilité de la VaR gaussienne comparativement à
la VaR empirique (historique) lorsque la distribution sous-jacente des rendements présente des queues
épaisses. Premièrement, simulez une seule série de rendements à partir d’une distribution de Student-t
à 3 degrés de liberté. Ensuite, en utilisant le rééchantillonnage bootstrap, générez de façon répétée
de nouveaux échantillons à partir de cette série de rendements et estimez à la fois la VaR gaussienne
et la VaR empirique à 5% pour chaque rééchantillon. Pour chaque méthode, calculez la proportion
de fois où l’estimation de la VaR est violée par les rendements originaux, et calculez la distorsion de
taille moyenne à travers les échantillons bootstrap. Quelle méthode fournit une couverture plus fiable?
Qu’est-ce que cela suggère quant au risque de modèle lors de l’application d’hypothèses gaussiennes à
des données à queues épaisses? [10 points]
Problème 4 [15 points], Combinaison de simulations et de valeur à
risque
Dansceproblème,vousévaluerezcommentlesestimationshistoriquesdelavaleuràrisque(VaR)évoluent
dansletempsetcommentceschangementspourraientêtreinterprétésparuncomitéderisquefinancier.Vous
travaillerez avec l’une des actions individuelles utilisées précédemment ou générerez de nouveaux rendements
synthétiques en utilisant une distribution de Student-tà 3 degrés de liberté pour simuler une série avec des
4

queues épaisses réalistes.
a.Présentezlesstatistiquessommairesdebase(moyenne,écart-type,asymétrie,aplatissement)pourvotre
sériederendementschoisie,etincluezdesgraphiquesdesérieschronologiquesbienétiquetésdesniveaux
de rendement. Si vous utilisez des données simulées, expliquez la structure du PGD. Commentez si la
distribution semble symétrique, à queues épaisses ou volatile dans le temps, et établissez brièvement
un lien entre vos résultats et ce que nous pourrions attendre en pratique des rendements d’actifs réels.
[3 points]
b.Calculez une VaR historique à 5% en utilisant une fenêtre mobile de 250 jours. Tracez la série chro-
nologique résultante de la VaR estimée aux côtés des rendements réalisés, et indiquez clairement où se
produisent les violations (c’est-à-dire où les rendements réels tombent en dessous de la VaR). Interpré-
tez le moment et le regroupement de ces violations. Y a-t-il des périodes où le modèle semble trop lent
à réagir? [4 points]
c.CalculezmaintenantlamêmeVaRhistoriqueà5%enutilisantunefenêtreexpansive(commençantavec
250 jours et augmentant d’une observation à chaque fois). Tracez les estimations de VaR résultantes
et comparez leur stabilité et leur réactivité aux estimations de la fenêtre mobile. Quelle méthode de
fenêtrage est plus conservatrice? Laquelle est plus sensible aux chocs récents? [4 points]
d.Supposez qu’on vous demande d’expliquer une augmentation récente des estimations de VaR à un
comité de risque, même si les rendements ont été en grande partie positifs dans le passé récent. Rédigez
une brève explication (environ 2 à 3 phrases) interprétant ce comportement en termes de volatilité
des rendements, de structure de fenêtre temporelle et de la logique sous-jacente aux mesures de risque
fondées sur les quantiles. Votre explication devrait refléter une compréhension claire de ce que le modèle
capture et de la façon dont cela pourrait être communiqué à des intervenants non techniques. [4 points]
5
