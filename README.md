# Projet du PFE

Demo link : https://drive.google.com/file/d/1vhp30ti2o3SypDs_5qj3cOWr5gBhEF7K/view?usp=drive_link


1. Contexte du projet

En Côte d'Ivoire, la prévalence et la mortalité du cancer sont des problèmes de santé publique importants. Selon les estimations de Globocan 2020, il y a eu 17 300 nouveaux cas en Côte d'Ivoire, dont 9896 femmes et 7404 hommes. Le cancer du sein est le plus fréquent de toutes les parties du corps et sexes confondues (19,1%), suivi du cancer de la prostate (15,9%), du cancer du col de l'utérus (11,9%), du cancer du foie (6,6%), et des lymphomes non hodgkiniens (4,9%). Les tumeurs les plus fréquemment diagnostiquées chez les femmes sont celles du sein et du col de l’utérus, avec des taux d'incidence standardisés de 44,7 et 31,2 respectivement pour 100 000 femmes. En outre, le taux de mortalité lié à la tumeur reste très élevé. En effet, les estimations pour 2020 situent le nombre de décès à environ 11 760. Ce nombre est en grande partie dû au diagnostic tardif dans approximativement 75 % des cas, le mauvais diagnostic et de la méconnaissance de la maladie cancéreuse. C’est dans ce contexte de résoudre ces problématiques de plus en plus inquiétantes que l’entreprise TIR, nous demande de proposer une solution d’aide à la détection du cancer du sein à partir des images de mammographies à l’aide de l’intelligence artificielle au sein de son logiciel de dossier patient informatisé.

2. Objectifs

L’objectif général de ce stage, c’est de mettre en place une application web au sein du DPI permettant le dépistage du cancer du sein à partir de la mammographie à l’aide des algorithmes d’intelligence artificielle. Pour y parvenir, nous déterminons cinq objectifs spécifiques du projet, à savoir :
  - collecter et préparer un ensemble de mammographies ;
  - déterminer les facteurs indiquant la présence d'un cancer du sein dans une
  mammographie ;
  - implémenter un modèle de détection du cancer du sein sur les images de
  mammographies ;
  - intégrer le système au sein du DPI ;
  - tester la fiabilité du système.

3. Présentation de notre approche
     
Pour la conception de notre modèle de vision par ordinateur, en nous appuyant sur les travaux de l'art de l'art. Nous optons pour des architectures implémentant des modèles préentraînés basés sur des réseaux de neurones de convolutions pour la détection du cancer. Puis, nous complétons en sortie de ceux- ci, des couches d’auto attentions, une couche de sortie suivie d’une carte d'activation de classe pondérée par le gradient. Elle permet de mettre en évidence les régions qui ont été pertinentes lors de la décision de notre modèle. Par elle, le radiologue peut avoir une segmentation visuelle de la zone de l’image abritant la tumeur. De plus, des techniques d'augmentation sont implémentées dans notre approche lors de l'entraînement de notre modèle, permettant ainsi de lutter contre le sur-apprentissage. Pour terminer, ces résultats sont implantés dans une plateforme ludique destinée aux radiologues.

4. Résultats
   
Cette méthodologie d’analyse suivie a produit les résultats escomptés. Notre solution se présente sous forme d’une application web intégrée au logiciel DPI, permettant aux radiologues d’effectuer le dépistage du cancer après avoir chargé des images mammaires produites par un mammographe. Puis, les résultats du diagnostic fournis par le modèle de VO sur la base des images entrées en arrière- plan, sont par la suite envoyés aux radiologues. Ce qui lui permet de délivrer un meilleur diagnostic et d’optimiser le temps de traitement lors de la prise en charge de ce dernier.
Cette solution s’avère pertinente et originale, car elle utilise des approches originales . Cependant, l’on peut l’améliorer. Une première perspective consiste à améliorer le score AUC-ROC de notre modèle de détection du cancer du sein, dans le but de passer de 85 % à 99 %. 
