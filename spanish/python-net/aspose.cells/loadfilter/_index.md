---
title: LoadFilter clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1010
url: /es/python-net/aspose.cells/loadfilter/
is_root: false
---
##  LoadFilter clase
Representa el filtro que proporciona opciones para cargar datos al cargar un libro de trabajo desde una plantilla.



El tipo LoadFilter expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [LoadFilter()](/cells/es/python-net/aspose.cells/loadfilter/__init__/#) | Construye un LoadFilter con opciones de filtro predeterminadas LoadDataFilterOptions.All.|
| [LoadFilter(opts)](/cells/es/python-net/aspose.cells/loadfilter/__init__/#LoadDataFilterOptions) | Construye un LoadFilter con opciones de filtro dadas.|


###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [load_data_filter_options](/cells/es/python-net/aspose.cells/loadfilter/load_data_filter_options) | Las opciones de filtro para indicar qué datos deben cargarse.|
| [sheets_in_loading_order](/cells/es/python-net/aspose.cells/loadfilter/sheets_in_loading_order) | Especifica las hojas (índices) y el orden en que se cargarán.<br/>El valor predeterminado es nulo, lo que indica cargar todas las hojas en el orden predeterminado en el archivo de plantilla.<br/> Si no es nulo y el índice de alguna hoja no está en la matriz devuelta, entonces la hoja no se cargará.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [start_sheet(sheet)](/cells/es/python-net/aspose.cells/loadfilter/start_sheet/#Worksheet) | Prepara las opciones de filtro antes de cargar la hoja de trabajo dada.<br/>La implementación del usuario de LoadFilter puede cambiar LoadDataFilterOptions aquí<br/> para indicar cómo cargar datos para esta hoja de cálculo.|



###  Observaciones

El usuario puede especificar las opciones de filtro o implementar su propio LoadFilter para especificar cómo cargar datos.

###  Ver también
* módulo [aspose.cells](..)
