---
title: ConditionalFormattingCollection
second_title: Referencia de API de Aspose.Cells para .NET
description: Encapsula una colección deFormatCondition./formatcondition objetos.
type: docs
weight: 1100
url: /es/net/aspose.cells/conditionalformattingcollection/
---
## ConditionalFormattingCollection class

Encapsula una colección de[`FormatCondition`](../formatcondition) objetos.

```csharp
public class ConditionalFormattingCollection : CollectionBase<FormatConditionCollection>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/conditionalformattingcollection/item) { get; } | Obtiene el elemento FormatConditions en el índice especificado. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells/conditionalformattingcollection/add)() | Agrega FormatConditions a la colección. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(FormatConditionCollection) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(FormatConditionCollection, IComparer&lt;FormatConditionCollection&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, FormatConditionCollection, IComparer&lt;FormatConditionCollection&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(FormatConditionCollection) |  |
| [Copy](../../aspose.cells/conditionalformattingcollection/copy)(ConditionalFormattingCollection) | Copia formato condicional. |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(FormatConditionCollection[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(FormatConditionCollection[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, FormatConditionCollection[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(FormatConditionCollection) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(FormatConditionCollection, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(FormatConditionCollection, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(FormatConditionCollection) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(FormatConditionCollection, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(FormatConditionCollection, int, int) |  |
| [RemoveArea](../../aspose.cells/conditionalformattingcollection/removearea)(int, int, int, int) | Eliminar todo el formato condicional en el rango. |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### Ejemplos

```csharp

[C#]

// Instanciando un objeto Workbook
Workbook workbook = new Workbook();

Worksheet sheet = workbook.Worksheets[0];

//Obtener formato condicional
ConditionalFormattingCollection cformattings = sheet.ConditionalFormattings;

//Agrega un formato condicional vacío
int index = cformattings.Add();

// Obtener el formato condicional recién agregado
FormatConditionCollection fcs = cformattings[index];

//Establece el rango de formato condicional.
CellArea ca = new CellArea();

ca.StartRow = 0;

ca.EndRow = 0;

ca.StartColumn = 0;

ca.EndColumn = 0;

fcs.AddArea(ca);

ca = new CellArea();

ca.StartRow = 1;

ca.EndRow = 1;

ca.StartColumn = 1;

ca.EndColumn = 1;

fcs.AddArea(ca);

//Añadir condición.
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");

//Añadir condición.
int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");

//Establece el color de fondo.
FormatCondition fc = fcs[conditionIndex];

fc.Style.BackgroundColor = Color.Red;

//Guardando el archivo de Excel
workbook.Save("output.xls");

[VB.NET]

'Crear una instancia de un objeto Workbook
DDim workbook As Workbook = New Workbook()

Dim sheet As Worksheet = workbook.Worksheets(0)

'Obtener formato condicional
Dim cformattings As ConditionalFormattingCollection = sheet.ConditionalFormattings

'Agrega un formato condicional vacío
Dim index As Integer = cformattings.Add()

'Obtenga el formato condicional recién agregado
Dim fcs As FormatConditionCollection = cformattings(index)

'Establece el rango de formato condicional.
Dim ca As New CellArea()

ca.StartRow = 0

ca.EndRow = 0

ca.StartColumn = 0

ca.EndColumn = 0

fcs.AddArea(ca)

ca = New CellArea()

ca.StartRow = 1

ca.EndRow = 1

ca.StartColumn = 1

ca.EndColumn = 1

fcs.AddArea(ca)

'Añadir condición.
Dim conditionIndex As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100")

'Añadir condición.
Dim conditionIndex2 As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100")

'Establece el color de fondo.
Dim fc As FormatCondition = fcs(conditionIndex)

fc.Style.BackgroundColor = Color.Red

'Guardar el archivo de Excel
workbook.Save("output.xls")
```

### Ver también

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [FormatConditionCollection](../formatconditioncollection)
* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
