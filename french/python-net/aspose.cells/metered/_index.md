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
Fournit des méthodes pour définir des clés mesurées.



Le type Metered expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [Metered()](/cells/fr/python-net/aspose.cells/metered/__init__/#) | Initialise une nouvelle instance de cette classe.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [set_metered_key(public_key, private_key)](/cells/fr/python-net/aspose.cells/metered/set_metered_key/#str-str) | Définit des clés publiques et privées mesurées.<br/>Si vous achetez une licence limitée, au démarrage de l'application, ce API doit être appelé, normalement, cela suffit. Vous devez vérifier régulièrement l'état de la licence, s'il s'agit d'un statut d'évaluation, appelez à nouveau ce API.|
| [get_consumption_quantity()](/cells/fr/python-net/aspose.cells/metered/get_consumption_quantity/#) | Obtient la taille du fichier de consommation|
| [get_consumption_credit()](/cells/fr/python-net/aspose.cells/metered/get_consumption_credit/#) | Obtient un crédit à la consommation|



###  Exemples

Dans cet exemple, une tentative sera faite pour définir des clés publiques et privées mesurées


```python
from aspose.cells import Metered

matered = Metered()
matered.set_metered_key("PublicKey", "PrivateKey")

```

###  Voir également
* module [aspose.cells](..)
