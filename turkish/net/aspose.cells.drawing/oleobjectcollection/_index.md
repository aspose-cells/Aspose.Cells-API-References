---
title: "Sınıf OleObjectCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.OleObjectCollection sınıfı. Gömülü OLE nesnelerini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/oleobjectcollection/
---
## OleObjectCollection class

Gömülü OLE nesnelerini temsil eder.

```csharp
public class OleObjectCollection : CollectionBase<OleObject>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/oleobjectcollection/item/) { get; } | Belirtilen indeksteki [`OleObject`](../oleobject/) öğesini alır. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells.drawing/oleobjectcollection/add/#add)(int, int, int, int, byte[]) | Koleksiyona bir OleObject ekler. |
| [Add](../../aspose.cells.drawing/oleobjectcollection/add/#add_1)(int, int, int, int, byte[], string) | Koleksiyona bağlı bir OleObject ekler. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(OleObject) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(OleObject, IComparer&lt;OleObject&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, OleObject, IComparer&lt;OleObject&gt;) |  |
| [Clear](../../aspose.cells.drawing/oleobjectcollection/clear/#clear)() | Tüm gömülü OLE nesnelerini kaldır. (2 yöntem) |
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
| [RemoveAt](../../aspose.cells.drawing/oleobjectcollection/removeat/#removeat)(int) | Belirtilen indeksteki öğeyi kaldırır. (2 yöntem) |

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı OLE nesneleri ekle
            int oleObjectIndex1 = worksheet.OleObjects.Add(10, 10, 100, 100, new byte[0]);
            int oleObjectIndex2 = worksheet.OleObjects.Add(50, 50, 100, 100, new byte[0]);

            // OleObjectCollection'ı al
            OleObjectCollection oleObjects = worksheet.OleObjects;

            // OLE nesneleri hakkında bilgi göster
            Console.WriteLine("OLE Objects Count: " + oleObjects.Count);
            for (int i = 0; i < oleObjects.Count; i++)
            {
                Console.WriteLine($"OLE Object {i + 1}:");
                Console.WriteLine($"- Position: ({oleObjects[i].UpperLeftRow}, {oleObjects[i].UpperLeftColumn})");
                Console.WriteLine($"- Size: {oleObjects[i].Width}x{oleObjects[i].Height}");
                Console.WriteLine($"- File: {oleObjects[i].FileFormatType}");
            }

            // İlk OLE nesnesini kaldır
            worksheet.OleObjects.RemoveAt(0);
            Console.WriteLine("\nAfter removing first OLE object:");
            Console.WriteLine("OLE Objects Count: " + oleObjects.Count);

            // Tüm OLE nesnelerini temizle
            worksheet.OleObjects.Clear();
            Console.WriteLine("\nAfter clearing all OLE objects:");
            Console.WriteLine("OLE Objects Count: " + oleObjects.Count);
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [OleObject](../oleobject/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


