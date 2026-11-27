---
title: "Klassen OleObjectCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.OleObjectCollection-klass. Representerar inbäddade OLE-objekt"
type: docs
url: /sv/net/aspose.cells.drawing/oleobjectcollection/
---
## OleObjectCollection class

Representerar inbäddade OLE-objekt.

```csharp
public class OleObjectCollection : CollectionBase<OleObject>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/oleobjectcollection/item/) { get; } | Hämtar [`OleObject`](../oleobject/) elementet på det angivna indexet. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.drawing/oleobjectcollection/add/#add)(int, int, int, int, byte[]) | Lägger till ett OleObject i samlingen. |
| [Add](../../aspose.cells.drawing/oleobjectcollection/add/#add_1)(int, int, int, int, byte[], string) | Lägger till ett länkat OleObject i samlingen. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(OleObject) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(OleObject, IComparer&lt;OleObject&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, OleObject, IComparer&lt;OleObject&gt;) |  |
| [Clear](../../aspose.cells.drawing/oleobjectcollection/clear/#clear)() | Ta bort alla inbäddade OLE-objekt. (2 metoder) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(OleObject) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(OleObject[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(OleObject[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, OleObject[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;OleObject&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;OleObject&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;OleObject&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;OleObject&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;OleObject&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;OleObject&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;OleObject&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;OleObject&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;OleObject&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;OleObject&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(OleObject) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(OleObject, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(OleObject, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(OleObject) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(OleObject, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(OleObject, int, int) |  |
| [RemoveAt](../../aspose.cells.drawing/oleobjectcollection/removeat/#removeat)(int) | Tar bort elementet på det angivna indexet. (2 metoder) |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassOleObjectCollectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till några OLE-objekt i kalkylbladet
            int oleObjectIndex1 = worksheet.OleObjects.Add(10, 10, 100, 100, new byte[0]);
            int oleObjectIndex2 = worksheet.OleObjects.Add(50, 50, 100, 100, new byte[0]);

            // Hämta OleObjectCollection
            OleObjectCollection oleObjects = worksheet.OleObjects;

            // Visa information om OLE-objekten
            Console.WriteLine("OLE Objects Count: " + oleObjects.Count);
            for (int i = 0; i < oleObjects.Count; i++)
            {
                Console.WriteLine($"OLE Object {i + 1}:");
                Console.WriteLine($"- Position: ({oleObjects[i].UpperLeftRow}, {oleObjects[i].UpperLeftColumn})");
                Console.WriteLine($"- Size: {oleObjects[i].Width}x{oleObjects[i].Height}");
                Console.WriteLine($"- File: {oleObjects[i].FileFormatType}");
            }

            // Ta bort det första OLE-objektet
            worksheet.OleObjects.RemoveAt(0);
            Console.WriteLine("\nAfter removing first OLE object:");
            Console.WriteLine("OLE Objects Count: " + oleObjects.Count);

            // Rensa alla OLE-objekt
            worksheet.OleObjects.Clear();
            Console.WriteLine("\nAfter clearing all OLE objects:");
            Console.WriteLine("OLE Objects Count: " + oleObjects.Count);
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [OleObject](../oleobject/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


