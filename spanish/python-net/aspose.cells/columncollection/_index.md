---
title: ColumnCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 270
url: /es/python-net/aspose.cells/columncollection/
is_root: false
---
##  ColumnCollection clase
Colección de los objetos [Column](/cells/es/python-net/aspose.cells/column) que representan las columnas individuales (configuraciones) en una hoja de cálculo.
El objeto Columna solo representa la configuración, como el ancho de columna, los estilos, etc. para toda la columna,
no tiene nada que ver con el hecho de que no hay celdas vacías (datos) o no en la columna correspondiente.
el "Recuento" de esta colección solo representa los objetos de columna de recuento que se han instanciado en esta colección,
no tiene nada que ver con el hecho de que no hay celdas vacías (datos) o no en la hoja de cálculo.



El tipo ColumnCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [capacity](/cells/es/python-net/aspose.cells/columncollection/capacity) | Obtiene o establece el número de elementos que puede contener la lista de matrices.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [copy_to(array)](/cells/es/python-net/aspose.cells/columncollection/copy_to/#list) | Copia toda la lista de matrices en una lista de matrices unidimensional compatible, comenzando por el principio de la lista de matrices de destino.|
| [copy_to(index, array, array_index, count)](/cells/es/python-net/aspose.cells/columncollection/copy_to/#int-list-int-int) | Copia un rango de elementos de la lista de arreglos a una lista de arreglos unidimensional compatible, comenzando en el índice especificado de la lista de arreglos de destino.|
| [index_of(item, index)](/cells/es/python-net/aspose.cells/columncollection/index_of/#Column-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el índice especificado hasta el último elemento.|
| [index_of(item, index, count)](/cells/es/python-net/aspose.cells/columncollection/index_of/#Column-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de matriz que comienza en el índice especificado y contiene el número especificado de elementos.|
| [last_index_of(item)](/cells/es/python-net/aspose.cells/columncollection/last_index_of/#Column) | Busca el objeto especificado y devuelve el índice de base cero de la última aparición en toda la lista de matrices.|
| [last_index_of(item, index)](/cells/es/python-net/aspose.cells/columncollection/last_index_of/#Column-int) |Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el primer elemento hasta el índice especificado.|
| [last_index_of(item, index, count)](/cells/es/python-net/aspose.cells/columncollection/last_index_of/#Column-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de matriz que contiene el número especificado de elementos y termina en el índice especificado.|
| [get_by_index(index)](/cells/es/python-net/aspose.cells/columncollection/get_by_index/#int) | Obtiene el objeto de la columna por el índice.|
| [get_column_by_index(index)](/cells/es/python-net/aspose.cells/columncollection/get_column_by_index/#int) | Obtiene el objeto [Column](/cells/es/python-net/aspose.cells/column) por la posición en la lista.|
| [binary_search(item)](/cells/es/python-net/aspose.cells/columncollection/binary_search/#Column) | Busca un elemento en toda la lista de matrices ordenadas mediante el comparador predeterminado y devuelve el índice de base cero del elemento.|



###  Ejemplo

```python
from aspose.cells import BackgroundType, StyleFlag, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Add new Style to Workbook
style = workbook.create_style()
# Setting the background color to Blue
style.foreground_color = Color.blue
# setting Background Pattern
style.pattern = BackgroundType.SOLID
# New Style Flag
styleFlag = StyleFlag()
# Set All Styles
styleFlag.all = True
# Change the default width of first ten columns
for i in range(10):
    worksheet.cells.columns[i].width = 20
# Get the Column with non default formatting
columns = worksheet.cells.columns
for column in columns:
    # Apply Style to first ten Columns
    column.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")

```

###  Ver también
* módulo [aspose.cells](..)
* clase [Column](/cells/es/python-net/aspose.cells/column)
