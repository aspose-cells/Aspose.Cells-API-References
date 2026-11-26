---
title: "Clase ConditionalFormattingCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ConditionalFormattingCollection. Encapsula una colección de objetos FormatCondition"
type: docs
url: /es/net/aspose.cells/conditionalformattingcollection/
---
## ConditionalFormattingCollection class

Encapsula una colección de objetos [`FormatCondition`](../formatcondition/).

```csharp
public class ConditionalFormattingCollection : CollectionBase<FormatConditionCollection>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/conditionalformattingcollection/item/) { get; } | Obtiene el elemento FormatConditions en el índice especificado. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells/conditionalformattingcollection/add/)() | Agrega un FormatConditions a la colección. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FormatConditionCollection) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FormatConditionCollection, IComparer&lt;FormatConditionCollection&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, FormatConditionCollection, IComparer&lt;FormatConditionCollection&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(FormatConditionCollection) |  |
| [Copy](../../aspose.cells/conditionalformattingcollection/copy/)(ConditionalFormattingCollection) | Copia el formato condicional. |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FormatConditionCollection[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FormatConditionCollection[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, FormatConditionCollection[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FormatConditionCollection) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FormatConditionCollection, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FormatConditionCollection, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FormatConditionCollection) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FormatConditionCollection, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FormatConditionCollection, int, int) |  |
| [RemoveArea](../../aspose.cells/conditionalformattingcollection/removearea/)(int, int, int, int) | Elimina todo el formato condicional en el rango. |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ConditionalFormattingCollectionDemo
    {
        public static void ConditionalFormattingCollectionExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Obtener formato condicional
            ConditionalFormattingCollection cformattings = sheet.ConditionalFormattings;

            // Agrega un formato condicional vacío
            int index = cformattings.Add();

            // Obtener el formato condicional recién añadido
            FormatConditionCollection fcs = cformattings[index];

            // Establece el rango del formato condicional.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 0,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            ca = new CellArea
            {
                StartRow = 1,
                EndRow = 1,
                StartColumn = 1,
                EndColumn = 1
            };
            fcs.AddArea(ca);

            // Agregar condición.
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");

            // Establece el color de fondo.
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            // Guardando el archivo Excel
            workbook.Save("ConditionalFormattingCollectionDemo.xlsx");
            workbook.Save("ConditionalFormattingCollectionDemo.pdf");
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [FormatConditionCollection](../formatconditioncollection/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


