---
title: "Clase ConditionalFormattingIconCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ConditionalFormattingIconCollection. Representa una colección de objetos ConditionalFormattingIcon."
type: docs
url: /es/net/aspose.cells/conditionalformattingiconcollection/
---
## ConditionalFormattingIconCollection class

Representa una colección de objetos [`ConditionalFormattingIcon`](../conditionalformattingicon/)

```csharp
public class ConditionalFormattingIconCollection : CollectionBase<ConditionalFormattingIcon>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/conditionalformattingiconcollection/item/) { get; } | Obtiene el elemento ConditionalFormattingIcon en el índice especificado. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells/conditionalformattingiconcollection/add/#add)(ConditionalFormattingIcon) | (**Obsoleto.**) Añade el objeto [`ConditionalFormattingIcon`](../conditionalformattingicon/). |
| [Add](../../aspose.cells/conditionalformattingiconcollection/add/#add_1)(IconSetType, int) | Añade el objeto [`ConditionalFormattingIcon`](../conditionalformattingicon/). |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ConditionalFormattingIcon) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ConditionalFormattingIcon, IComparer&lt;ConditionalFormattingIcon&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ConditionalFormattingIcon, IComparer&lt;ConditionalFormattingIcon&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ConditionalFormattingIcon) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ConditionalFormattingIcon[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ConditionalFormattingIcon[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ConditionalFormattingIcon[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConditionalFormattingIcon) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConditionalFormattingIcon, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConditionalFormattingIcon, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConditionalFormattingIcon) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConditionalFormattingIcon, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConditionalFormattingIcon, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingIconCollectionDemo
    {
        public static void ConditionalFormattingIconCollectionExample()
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

            // Establece la condición
            int idx = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[idx];

            // Establece el tipo de la condición
            cond.IconSet.Type = IconSetType.ArrowsGray3;

            // Añade una condición de iconset personalizada.
            ConditionalFormattingIcon cfIcon = cond.IconSet.CfIcons[0];
            cfIcon.Type = IconSetType.Arrows3;
            cfIcon.Index = 0;

            ConditionalFormattingIcon cfIcon1 = cond.IconSet.CfIcons[1];
            cfIcon1.Type = IconSetType.ArrowsGray3;
            cfIcon1.Index = 1;

            ConditionalFormattingIcon cfIcon2 = cond.IconSet.CfIcons[2];
            cfIcon2.Type = IconSetType.Boxes5;
            cfIcon2.Index = 2;

            // Guardando el archivo Excel
            workbook.Save("outConditionalFormattingIconCollectionDemoput.xlsx");
            workbook.Save("outConditionalFormattingIconCollectionDemoput.pdf");
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ConditionalFormattingIcon](../conditionalformattingicon/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


