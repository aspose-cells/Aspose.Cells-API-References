---
title: classe ExternalConnectionCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 60
url: /it/python-net/aspose.cells.externalconnections/externalconnectioncollection/
is_root: false
---
##  classe ExternalConnectionCollection
Specifica la raccolta [ExternalConnection](/cells/it/python-net/aspose.cells.externalconnections/externalconnection)



Il tipo ExternalConnectionCollection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [capacity](/cells/it/python-net/aspose.cells.externalconnections/externalconnectioncollection/capacity) | Ottiene o imposta il numero di elementi che l'elenco di matrici può contenere.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [copy_to(array)](/cells/it/python-net/aspose.cells.externalconnections/externalconnectioncollection/copy_to/#list) | Copia l'intero elenco di matrici in un elenco di matrici unidimensionale compatibile, a partire dall'inizio dell'elenco di matrici di destinazione.|
| [copy_to(index, array, array_index, count)](/cells/it/python-net/aspose.cells.externalconnections/externalconnectioncollection/copy_to/#int-list-int-int) |Copia un intervallo di elementi dall'elenco di matrici a un elenco di matrici unidimensionale compatibile, a partire dall'indice specificato dell'elenco di matrici di destinazione.|
| [index_of(item, index)](/cells/it/python-net/aspose.cells.externalconnections/externalconnectioncollection/index_of/#ExternalConnection-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dall'indice specificato all'ultimo elemento.|
| [index_of(item, index, count)](/cells/it/python-net/aspose.cells.externalconnections/externalconnectioncollection/index_of/#ExternalConnection-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che inizia dall'indice specificato e contiene il numero specificato di elementi.|
| [last_index_of(item)](/cells/it/python-net/aspose.cells.externalconnections/externalconnectioncollection/last_index_of/#ExternalConnection) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intero elenco di matrici.|
| [last_index_of(item, index)](/cells/it/python-net/aspose.cells.externalconnections/externalconnectioncollection/last_index_of/#ExternalConnection-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dal primo elemento all'indice specificato.|
| [last_index_of(item, index, count)](/cells/it/python-net/aspose.cells.externalconnections/externalconnectioncollection/last_index_of/#ExternalConnection-int-int) |Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che contiene il numero specificato di elementi e termina con l'indice specificato.|
| [get_external_connection_by_id(conn_id)](/cells/it/python-net/aspose.cells.externalconnections/externalconnectioncollection/get_external_connection_by_id/#int) | Ottiene l'elemento [ExternalConnection](/cells/it/python-net/aspose.cells.externalconnections/externalconnection) con l'ID specificato.|
| [binary_search(item)](/cells/it/python-net/aspose.cells.externalconnections/externalconnectioncollection/binary_search/#ExternalConnection) | Cerca un elemento nell'intero elenco di matrici ordinate utilizzando l'operatore di confronto predefinito e restituisce l'indice in base zero dell'elemento.|



###  Esempio

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

###  Guarda anche
* modulo [aspose.cells.externalconnections](..)
* classe [ExternalConnection](/cells/it/python-net/aspose.cells.externalconnections/externalconnection)
