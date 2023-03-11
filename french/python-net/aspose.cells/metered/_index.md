---
title: Metered classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1050
url: /fr/python-net/aspose.cells/metered/
is_root: false
---
##  Metered classe
Fournit des méthodes pour définir une clé mesurée.



Le type Metered expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [Metered()](/cells/fr/python-net/aspose.cells/metered/__init__/#) | Initialise une nouvelle instance de cette classe.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [set_metered_key(public_key, private_key)](/cells/fr/python-net/aspose.cells/metered/set_metered_key/#str-str) | Définit une clé publique et privée mesurée.<br/>Si vous achetez une licence limitée, lorsque vous démarrez l'application, ce API doit être appelé, normalement, cela suffit. Cependant, si vous ne parvenez toujours pas à télécharger les données de consommation et dépassez 24 heures, la licence sera définie sur le statut d'évaluation. Pour éviter ce cas, vous devez vérifier régulièrement l'état de la licence. S'il s'agit d'un statut d'évaluation, appelez à nouveau ce API.|
| [get_consumption_quantity()](/cells/fr/python-net/aspose.cells/metered/get_consumption_quantity/#) | Obtient la taille du fichier de consommation|
| [get_consumption_credit()](/cells/fr/python-net/aspose.cells/metered/get_consumption_credit/#) | Obtient un crédit à la consommation|



###  Exemple

Dans cet exemple, une tentative sera faite pour définir des clés publiques et privées mesurées


```python
from aspose.cells import Metered

matered = Metered()
matered.set_metered_key("PublicKey", "PrivateKey")

```

###  Voir également
* module [aspose.cells](..)
