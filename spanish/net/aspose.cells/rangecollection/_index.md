---
title: "Clase RangeCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.RangeCollection. Encapsula una colección de objetos Range"
type: docs
url: /es/net/aspose.cells/rangecollection/
---
## RangeCollection class

Encapsula una colección de objetos [`Range`](../range/).

```csharp
public class RangeCollection : CollectionBase<Range>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/rangecollection/item/) { get; } | Obtiene el elemento [`Range`](../range/) en el índice especificado. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells/rangecollection/add/)(Range) | (**Obsolete.**) Agrega un elemento [`Range`](../range/) a la colección. |
| [AddRange](../../aspose.cells/rangecollection/addrange/)(Range) | Agrega un elemento [`Range`](../range/) a la colección. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Range) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Range, IComparer&lt;Range&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Range, IComparer&lt;Range&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Range) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Range[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Range[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Range[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Range&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Range&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Range&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Range&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Range&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Range&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Range&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Range&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Range&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Range&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Range) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Range, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Range, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Range) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Range, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Range, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassRangeCollectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear rangos y agregarlos a la hoja de cálculo
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C3:D4");
            
            // Obtener el RangeCollection de la hoja de cálculo
            RangeCollection rangeCollection = worksheet.Cells.Ranges;
            
            // Agregar rangos a la colección
            rangeCollection.Add(range1);
            rangeCollection.Add(range2);

            // Crear otro RangeCollection para comparación
            RangeCollection compareCollection = worksheet.Cells.Ranges;
            compareCollection.Add(worksheet.Cells.CreateRange("A1:B2"));
            compareCollection.Add(worksheet.Cells.CreateRange("C3:D4"));

            // Comparar los dos RangeCollections
            bool areEqual = CompareRangeCollections(rangeCollection, compareCollection);
            Console.WriteLine("RangeCollections are equal: " + areEqual);
        }

        private static bool CompareRangeCollections(RangeCollection src, RangeCollection dest)
        {
            if (src.Count != dest.Count)
                return false;

            for (int i = 0; i < src.Count; i++)
            {
                bool foundMatch = false;
                Aspose.Cells.Range srcRange = src[i];
                
                foreach (Aspose.Cells.Range destRange in dest)
                {
                    if (srcRange.FirstRow == destRange.FirstRow &&
                        srcRange.FirstColumn == destRange.FirstColumn &&
                        srcRange.RowCount == destRange.RowCount &&
                        srcRange.ColumnCount == destRange.ColumnCount)
                    {
                        foundMatch = true;
                        break;
                    }
                }
                
                if (!foundMatch)
                    return false;
            }
            
            return true;
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Range](../range/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


