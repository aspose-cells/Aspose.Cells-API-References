---
title: ExternalConnectionCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 60
url: /es/python-net/aspose.cells.externalconnections/externalconnectioncollection/
is_root: false
---
##  ExternalConnectionCollection clase
Especifica la colección [ExternalConnection](/cells/es/python-net/aspose.cells.externalconnections/externalconnection)



El tipo ExternalConnectionCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [capacity](/cells/es/python-net/aspose.cells.externalconnections/externalconnectioncollection/capacity) | Obtiene o establece el número de elementos que puede contener la lista de matrices.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [copy_to(array)](/cells/es/python-net/aspose.cells.externalconnections/externalconnectioncollection/copy_to/#list) | Copia toda la lista de matrices en una lista de matrices unidimensional compatible, comenzando por el principio de la lista de matrices de destino.|
| [copy_to(index, array, array_index, count)](/cells/es/python-net/aspose.cells.externalconnections/externalconnectioncollection/copy_to/#int-list-int-int) | Copia un rango de elementos de la lista de arreglos a una lista de arreglos unidimensional compatible, comenzando en el índice especificado de la lista de arreglos de destino.|
| [index_of(item, index)](/cells/es/python-net/aspose.cells.externalconnections/externalconnectioncollection/index_of/#ExternalConnection-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el índice especificado hasta el último elemento.|
| [index_of(item, index, count)](/cells/es/python-net/aspose.cells.externalconnections/externalconnectioncollection/index_of/#ExternalConnection-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de matriz que comienza en el índice especificado y contiene el número especificado de elementos.|
| [last_index_of(item)](/cells/es/python-net/aspose.cells.externalconnections/externalconnectioncollection/last_index_of/#ExternalConnection) | Busca el objeto especificado y devuelve el índice de base cero de la última aparición en toda la lista de matrices.|
| [last_index_of(item, index)](/cells/es/python-net/aspose.cells.externalconnections/externalconnectioncollection/last_index_of/#ExternalConnection-int) |Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el primer elemento hasta el índice especificado.|
| [last_index_of(item, index, count)](/cells/es/python-net/aspose.cells.externalconnections/externalconnectioncollection/last_index_of/#ExternalConnection-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de matriz que contiene el número especificado de elementos y termina en el índice especificado.|
| [get_external_connection_by_id(conn_id)](/cells/es/python-net/aspose.cells.externalconnections/externalconnectioncollection/get_external_connection_by_id/#int) | Obtiene el elemento [ExternalConnection](/cells/es/python-net/aspose.cells.externalconnections/externalconnection) con la identificación especificada.|
| [binary_search(item)](/cells/es/python-net/aspose.cells.externalconnections/externalconnectioncollection/binary_search/#ExternalConnection) | Busca un elemento en toda la lista de matrices ordenadas mediante el comparador predeterminado y devuelve el índice de base cero del elemento.|



###  Ejemplo

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

###  Ver también
* módulo [aspose.cells.externalconnections](..)
* clase [ExternalConnection](/cells/es/python-net/aspose.cells.externalconnections/externalconnection)
