---
title: ExternalConnectionCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 60
url: /fr/python-net/aspose.cells.externalconnections/externalconnectioncollection/
is_root: false
---
##  ExternalConnectionCollection classe
Spécifie la collection [ExternalConnection](/cells/fr/python-net/aspose.cells.externalconnections/externalconnection)



Le type ExternalConnectionCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [capacity](/cells/fr/python-net/aspose.cells.externalconnections/externalconnectioncollection/capacity) | Obtient ou définit le nombre d'éléments que la liste de tableau peut contenir.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [copy_to(array)](/cells/fr/python-net/aspose.cells.externalconnections/externalconnectioncollection/copy_to/#list) | Copie la totalité de la liste de tableaux dans une liste de tableaux unidimensionnelle compatible, en commençant au début de la liste de tableaux cible.|
| [copy_to(index, array, array_index, count)](/cells/fr/python-net/aspose.cells.externalconnections/externalconnectioncollection/copy_to/#int-list-int-int) |Copie une plage d'éléments de la liste de tableaux vers une liste de tableaux unidimensionnelle compatible, en commençant à l'index spécifié de la liste de tableaux cible.|
| [index_of(item, index)](/cells/fr/python-net/aspose.cells.externalconnections/externalconnectioncollection/index_of/#ExternalConnection-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui s'étend de l'index spécifié au dernier élément.|
| [index_of(item, index, count)](/cells/fr/python-net/aspose.cells.externalconnections/externalconnectioncollection/index_of/#ExternalConnection-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui commence à l'index spécifié et contient le nombre d'éléments spécifié.|
| [last_index_of(item)](/cells/fr/python-net/aspose.cells.externalconnections/externalconnectioncollection/last_index_of/#ExternalConnection) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la liste complète du tableau.|
| [last_index_of(item, index)](/cells/fr/python-net/aspose.cells.externalconnections/externalconnectioncollection/last_index_of/#ExternalConnection-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui s'étend du premier élément à l'index spécifié.|
| [last_index_of(item, index, count)](/cells/fr/python-net/aspose.cells.externalconnections/externalconnectioncollection/last_index_of/#ExternalConnection-int-int) |Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui contient le nombre d'éléments spécifié et se termine à l'index spécifié.|
| [get_external_connection_by_id(conn_id)](/cells/fr/python-net/aspose.cells.externalconnections/externalconnectioncollection/get_external_connection_by_id/#int) | Obtient l'élément [ExternalConnection](/cells/fr/python-net/aspose.cells.externalconnections/externalconnection) avec l'ID spécifié.|
| [binary_search(item)](/cells/fr/python-net/aspose.cells.externalconnections/externalconnectioncollection/binary_search/#ExternalConnection) | Recherche un élément dans toute la liste de tableaux triés à l'aide du comparateur par défaut et renvoie l'index de base zéro de l'élément.|



###  Exemple

```python
from aspose.cells import Workbook

wb = Workbook("connection.xlsx")
dataConns = wb.data_connections
dataConn = None
for i in range(len(dataConns)):
    dataConn = dataConns[i]
    # get external connection id
    print(dataConn.connection_id)

```

###  Voir également
* module [aspose.cells.externalconnections](..)
* classe [ExternalConnection](/cells/fr/python-net/aspose.cells.externalconnections/externalconnection)
