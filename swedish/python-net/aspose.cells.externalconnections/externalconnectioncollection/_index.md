---
title: ExternalConnectionCollection klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 60
url: /sv/python-net/aspose.cells.externalconnections/externalconnectioncollection/
is_root: false
---
##  ExternalConnectionCollection klass
Anger samlingen [ExternalConnection](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection)



Typen ExternalConnectionCollection avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [capacity](/cells/sv/python-net/aspose.cells.externalconnections/externalconnectioncollection/capacity) | Hämtar eller ställer in antalet element som arraylistan kan innehålla.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [copy_to(array)](/cells/sv/python-net/aspose.cells.externalconnections/externalconnectioncollection/copy_to/#list) | Kopierar hela arraylistan till en kompatibel endimensionell arraylista, med början i början av målarraylistan.|
| [copy_to(index, array, array_index, count)](/cells/sv/python-net/aspose.cells.externalconnections/externalconnectioncollection/copy_to/#int-list-int-int) |Kopierar ett intervall av element från arraylistan till en kompatibel endimensionell arraylista, med början vid det angivna indexet för målarraylistan.|
| [index_of(item, index)](/cells/sv/python-net/aspose.cells.externalconnections/externalconnectioncollection/index_of/#ExternalConnection-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som sträcker sig från det angivna indexet till det sista elementet.|
| [index_of(item, index, count)](/cells/sv/python-net/aspose.cells.externalconnections/externalconnectioncollection/index_of/#ExternalConnection-int-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som börjar vid det angivna indexet och innehåller det angivna antalet element.|
| [last_index_of(item)](/cells/sv/python-net/aspose.cells.externalconnections/externalconnectioncollection/last_index_of/#ExternalConnection) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom hela arraylistan.|
| [last_index_of(item, index)](/cells/sv/python-net/aspose.cells.externalconnections/externalconnectioncollection/last_index_of/#ExternalConnection-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som sträcker sig från det första elementet till det angivna indexet.|
| [last_index_of(item, index, count)](/cells/sv/python-net/aspose.cells.externalconnections/externalconnectioncollection/last_index_of/#ExternalConnection-int-int) |Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som innehåller det angivna antalet element och slutar vid det angivna indexet.|
| [get_external_connection_by_id(conn_id)](/cells/sv/python-net/aspose.cells.externalconnections/externalconnectioncollection/get_external_connection_by_id/#int) | Hämtar elementet [ExternalConnection](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection) med angivet ID.|
| [binary_search(item)](/cells/sv/python-net/aspose.cells.externalconnections/externalconnectioncollection/binary_search/#ExternalConnection) | Söker i hela den sorterade arraylistan efter ett element med hjälp av standardjämföraren och returnerar elementets nollbaserade index.|



###  Exempel

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

###  Se även
* modul [aspose.cells.externalconnections](..)
* klass [ExternalConnection](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection)
