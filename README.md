# SwAV - Swapping Assignments between Views
SwAV Implementaion Code

README https://github.com/facebookresearch/swav 
# Unsupervised Learning of Visual Features by Contrasting Cluster Assignments
Dieser Code bietet eine PyTorch-Implementierung und vortrainierte Modelle für **SwAV** (**Sw**apping **A**ssignments between **V**iews), wie im Paper [Unsupervised Learning of Visual Features by Contrasting Cluster Assignments](https://arxiv.org/abs/2006.09882) beschrieben .

<div align="center">
  <img width="100%" alt="SwAV Illustration" src="https://dl.fbaipublicfiles.com/deepcluster/animated.gif">
</div>

SwAV ist eine effiziente und einfache Methode zum Vortraining von Convnets ohne Verwendung von Annotationen.
Ähnlich wie bei kontrastiven Ansätzen lernt SwAV Repräsentationen durch den Vergleich von Transformationen eines Bildes, aber im Gegensatz zu kontrastiven Methoden ist es nicht erforderlich, paarweise Feature-Vergleiche zu berechnen.
Das macht unser Framework effizienter, da es weder eine große Speicherbank noch ein zusätzliches Impulsnetzwerk benötigt.
Unsere Methode clustert die Daten gleichzeitig und erzwingt dabei die Konsistenz zwischen den Cluster-Zuordnungen, die für verschiedene Augmentierungen (oder "Ansichten") desselben Bildes erzeugt werden, anstatt die Merkmale direkt zu vergleichen.
Einfach ausgedrückt, verwenden wir einen "vertauschten" Vorhersagemechanismus, bei dem wir die Clusterzuordnung einer Ansicht aus der Darstellung einer anderen Ansicht vorhersagen.
Unsere Methode kann mit großen und kleinen Stapeln trainiert werden und lässt sich auf unbegrenzte Datenmengen skalieren.

# Programmcode
Der zugrundeliegende Programmcode wurde von den Autoren übernommen. https://github.com/PyTorchLightning/pytorch-lightning-bolts.git

Code ist über PyTorchLightning umgesetzt. Zum starten des Notebooks einfach [swav.ipynb](./swav.ipynb) üer Google Colab öffen.

