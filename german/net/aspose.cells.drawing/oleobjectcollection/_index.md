---
title: "Klasse OleObjectCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.OleObjectCollection Klasse. Stellt eingebettete OLE-Objekte dar"
type: docs
url: /de/net/aspose.cells.drawing/oleobjectcollection/
---
## OleObjectCollection class

Stellt eingebettete OLE-Objekte dar.

```csharp
public class OleObjectCollection : CollectionBase<OleObject>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/oleobjectcollection/item/) { get; } | Ruft das [`OleObject`](../oleobject/) Element am angegebenen Index ab. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.drawing/oleobjectcollection/add/#add)(int, int, int, int, byte[]) | Fügt ein OleObject zur Sammlung hinzu. |
| [Add](../../aspose.cells.drawing/oleobjectcollection/add/#add_1)(int, int, int, int, byte[], string) | Fügt ein verknüpftes OleObject zur Sammlung hinzu. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(OleObject) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(OleObject, IComparer&lt;OleObject&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, OleObject, IComparer&lt;OleObject&gt;) |  |
| [Clear](../../aspose.cells.drawing/oleobjectcollection/clear/#clear)() | Entfernt alle eingebetteten OLE-Objekte. (2 Methoden) |
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
| [RemoveAt](../../aspose.cells.drawing/oleobjectcollection/removeat/#removeat)(int) | Entfernt das Element am angegebenen Index. (2 Methoden) |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige OLE-Objekte zum Arbeitsblatt hinzu
            int oleObjectIndex1 = worksheet.OleObjects.Add(10, 10, 100, 100, new byte[0]);
            int oleObjectIndex2 = worksheet.OleObjects.Add(50, 50, 100, 100, new byte[0]);

            // Rufen Sie die OleObjectCollection ab
            OleObjectCollection oleObjects = worksheet.OleObjects;

            // Informationen zu den OLE-Objekten anzeigen
            Console.WriteLine("OLE Objects Count: " + oleObjects.Count);
            for (int i = 0; i < oleObjects.Count; i++)
            {
                Console.WriteLine($"OLE Object {i + 1}:");
                Console.WriteLine($"- Position: ({oleObjects[i].UpperLeftRow}, {oleObjects[i].UpperLeftColumn})");
                Console.WriteLine($"- Size: {oleObjects[i].Width}x{oleObjects[i].Height}");
                Console.WriteLine($"- File: {oleObjects[i].FileFormatType}");
            }

            // Das erste OLE-Objekt entfernen
            worksheet.OleObjects.RemoveAt(0);
            Console.WriteLine("\nAfter removing first OLE object:");
            Console.WriteLine("OLE Objects Count: " + oleObjects.Count);

            // Alle OLE-Objekte löschen
            worksheet.OleObjects.Clear();
            Console.WriteLine("\nAfter clearing all OLE objects:");
            Console.WriteLine("OLE Objects Count: " + oleObjects.Count);
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [OleObject](../oleobject/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


