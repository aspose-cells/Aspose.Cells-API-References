---
title: "OleObjectCollection.RemoveAt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OleObjectCollection yöntemi. Belirtilen indeksteki öğeyi kaldırır"
type: docs
url: /tr/net/aspose.cells.drawing/oleobjectcollection/removeat/
---
## OleObjectCollection.RemoveAt method

Belirtilen indeksteki öğeyi kaldırır.

```csharp
public void RemoveAt(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Belirtilen indeks. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = workbook.Worksheets[0];
            
            // Örnek OLE nesneleri ekleyin (3 nesne)
            for (int i = 0; i < 3; i++)
            {
                sheet.OleObjects.Add(i * 10, i * 10, 100, 100, new byte[0]);
            }

            Console.WriteLine("Before removal - OLE Objects count: " + sheet.OleObjects.Count);
            
            // OLE nesnelerini tek tek RemoveAt(int index) kullanarak kaldırın
            for (int i = sheet.OleObjects.Count - 1; i >= 0; i--)
            {
                sheet.OleObjects.RemoveAt(i);
            }

            Console.WriteLine("After removal - OLE Objects count: " + sheet.OleObjects.Count);
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


