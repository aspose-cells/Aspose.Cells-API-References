---
title: ConditionalFormattingIconCollection
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa una colección deConditionalFormattingIcon./conditionalformattingicon objetos.
type: docs
weight: 1120
url: /es/net/aspose.cells/conditionalformattingiconcollection/
---
## ConditionalFormattingIconCollection class

Representa una colección de[`ConditionalFormattingIcon`](../conditionalformattingicon) objetos.

```csharp
public class ConditionalFormattingIconCollection : CollectionBase<ConditionalFormattingIcon>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/conditionalformattingiconcollection/item) { get; } | Obtiene el elemento ConditionalFormattingIcon en el índice especificado. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells/conditionalformattingiconcollection/add#add)(ConditionalFormattingIcon) | Agrega[`ConditionalFormattingIcon`](../conditionalformattingicon) objeto. |
| [Add](../../aspose.cells/conditionalformattingiconcollection/add#add_1)(IconSetType, int) | Agrega[`ConditionalFormattingIcon`](../conditionalformattingicon) objeto. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(ConditionalFormattingIcon) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(ConditionalFormattingIcon, IComparer&lt;ConditionalFormattingIcon&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, ConditionalFormattingIcon, IComparer&lt;ConditionalFormattingIcon&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(ConditionalFormattingIcon) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(ConditionalFormattingIcon[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(ConditionalFormattingIcon[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, ConditionalFormattingIcon[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(ConditionalFormattingIcon) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(ConditionalFormattingIcon, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(ConditionalFormattingIcon, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(ConditionalFormattingIcon) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(ConditionalFormattingIcon, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(ConditionalFormattingIcon, int, int) |  |
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

// Establece la condición
 int idx = fcs.AddCondition(FormatConditionType.IconSet);
 
 FormatCondition cond = fcs[idx];
   
 // Establece la condición's type
 cond.IconSet.Type = IconSetType.ArrowsGray3;

// Agregar condición de conjunto de iconos personalizado.
 ConditionalFormattingIcon cfIcon = cond.IconSet.CfIcons[0];
 
 cfIcon.Type = IconSetType.Arrows3;
 
 cfIcon.Index = 0;
 
 ConditionalFormattingIcon cfIcon1 = cond.IconSet.CfIcons[1];
 
  cfIcon1.Type = IconSetType.ArrowsGray3;
  
  cfIcon1.Index = 1;
  
  ConditionalFormattingIcon cfIcon2 = cond.IconSet.CfIcons[2];
  
  cfIcon2.Type = IconSetType.Boxes5;
  
  cfIcon2.Index = 2;

//Guardando el archivo de Excel
workbook.Save("output.xls");

[VB.NET]

'Crear una instancia de un objeto Workbook
Dim workbook As Workbook = New Workbook()

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

// Establece la condición
Dim idx As Integer =fcs.AddCondition(FormatConditionType.IconSet)

Dim cond As FormatCondition=fcs[idx]

// Establece la condición's type
cfIcon.Type = IconSetType.ArrowsGray3

'Agregue una condición de conjunto de iconos personalizado.
Dim cfIcon As ConditionalFormattingIcon = cond.IconSet.CfIcons[0]

cfIcon.Type = IconSetType.Arrows3

cfIcon.Index=0

Dim cfIcon1 As ConditionalFormattingIcon = cond.IconSet.CfIcons[1]

cfIcon1.Type = IconSetType.ArrowsGray3

cfIcon1.Index=1

Dim cfIcon2 As ConditionalFormattingIcon = cond.IconSet.CfIcons[2]

cfIcon2.Type = IconSetType.Boxes5

cfIcon2.Index=2

'Guardar el archivo de Excel
workbook.Save("output.xls")
```

### Ver también

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [ConditionalFormattingIcon](../conditionalformattingicon)
* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
