---
title: DataSorter
second_title: Referencia de API de Aspose.Cells para .NET
description: Descripción resumida para DataSorter.
type: docs
weight: 1300
url: /es/net/aspose.cells/datasorter/
---
## DataSorter class

Descripción resumida para DataSorter.

```csharp
public class DataSorter
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CaseSensitive](../../aspose.cells/datasorter/casesensitive) { get; set; } | Obtiene y establece si distingue entre mayúsculas y minúsculas al comparar cadenas. |
| [HasHeaders](../../aspose.cells/datasorter/hasheaders) { get; set; } | Representa si el rango tiene encabezados. |
| [Key1](../../aspose.cells/datasorter/key1) { get; set; } | Representa el índice de la primera columna ordenada (posición absoluta, la columna A es 0, B es 1, ...). |
| [Key2](../../aspose.cells/datasorter/key2) { get; set; } | Representa el índice de la segunda columna ordenada (posición absoluta, la columna A es 0, B es 1, ...). |
| [Key3](../../aspose.cells/datasorter/key3) { get; set; } | Representa el índice de la tercera columna ordenada (posición absoluta, la columna A es 0, B es 1, ...). |
| [Keys](../../aspose.cells/datasorter/keys) { get; } | Obtiene la lista de claves del clasificador de datos. |
| [Order1](../../aspose.cells/datasorter/order1) { get; set; } | Representa el orden de clasificación de la primera clave. |
| [Order2](../../aspose.cells/datasorter/order2) { get; set; } | Representa el orden de clasificación de la segunda clave. |
| [Order3](../../aspose.cells/datasorter/order3) { get; set; } | Representa el orden de clasificación de la tercera clave. |
| [SortAsNumber](../../aspose.cells/datasorter/sortasnumber) { get; set; } | Indica si ordenar cualquier cosa que parezca un número. |
| [SortLeftToRight](../../aspose.cells/datasorter/sortlefttoright) { get; set; } | Verdadero significa que la orientación de clasificación es de izquierda a derecha. Falso significa que la orientación de clasificación es de arriba a abajo. El valor predeterminado es falso. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey_1)(int, SortOrder) | Agrega índice de columna ordenada y orden de clasificación. |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey_2)(int, SortOrder, string) | Agrega índice de columna ordenado y orden de clasificación con lista de ordenación personalizada. |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey_3)(int, SortOrder, string[]) | Agrega índice de columna ordenado y orden de clasificación con lista de ordenación personalizada. |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey)(int, SortOnType, SortOrder, object) | Agrega índice de columna ordenado y orden de clasificación con lista de ordenación personalizada. |
| [Clear](../../aspose.cells/datasorter/clear)() | Borrar todas las configuraciones. |
| [Sort](../../aspose.cells/datasorter/sort#sort)() | Ordenar los datos en el rango. |
| [Sort](../../aspose.cells/datasorter/sort#sort_1)(Cells, CellArea) | Ordenar los datos del área. |
| [Sort](../../aspose.cells/datasorter/sort#sort_2)(Cells, int, int, int, int) | Ordena los datos del área. |

### Ejemplos

```csharp

[C#]

//Crea una instancia de un nuevo objeto Workbook.
Workbook workbook = new Workbook("Book1.xls");
//Obtenga el objeto del clasificador de datos del libro de trabajo.
DataSorter sorter = workbook.DataSorter;
//Establecer el primer orden para el objeto clasificador de datos.
sorter.Order1 = Aspose.Cells.SortOrder.Descending;
//Definir la primera clave.
sorter.Key1 = 0;
//Establecer el segundo orden para el objeto clasificador de datos.
sorter.Order2 = Aspose.Cells.SortOrder.Ascending;
//Defina la segunda clave.
sorter.Key2 = 1;
//Crear un área de celdas (rango).
CellArea ca = new CellArea();
//Especifique el índice de la fila de inicio.
ca.StartRow = 0;
//Especifique el índice de la columna de inicio.
ca.StartColumn = 0;
//Especifique el índice de la última fila.
ca.EndRow = 13;
//Especifique el índice de la última columna.
ca.EndColumn = 1;
//Ordenar datos en el rango de datos especificado (A1:B14)
sorter.Sort(workbook.Worksheets[0].Cells, ca);
//Guardar el archivo de Excel.
workbook.Save("outBook.xls");

[Visual Basic]

'Crea una instancia de un nuevo objeto Workbook.
Dim workbook As Workbook = New Workbook("Book1.xls")
'Obtenga el objeto del clasificador de datos del libro de trabajo.
Dim sorter As DataSorter = workbook.DataSorter
'Establecer el primer orden para el objeto clasificador de datos
sorter.Order1 = Aspose.Cells.SortOrder.Descending
'Defina la primera clave.
sorter.Key1 = 0
'Establezca el segundo orden para el objeto clasificador de datos.
sorter.Order2 = Aspose.Cells.SortOrder.Ascending
'Defina la segunda clave.
sorter.Key2 = 1
'Crea un área de celdas (rango).
Dim ca As CellArea = New CellArea
'Especifique el índice de la fila de inicio.
ca.StartRow = 0
'Especifique el índice de la columna de inicio.
ca.StartColumn = 0
'Especifique el índice de la última fila.
ca.EndRow = 13
'Especifique el índice de la última columna.
ca.EndColumn = 1
'Ordenar los datos en el rango de datos especificado (A1:B14)
sorter.Sort(workbook.Worksheets(0).Cells, ca)
'Guarde el archivo de Excel.
workbook.Save("outBook.xls")

```

### Ver también

* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
