---
title: "Worksheet.OleObjects"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Bir çalışma sayfasındaki OleObject koleksiyonunu temsil eder"
type: docs
url: /tr/net/aspose.cells/worksheet/oleobjects/
---
## Worksheet.OleObjects property

Bir çalışma sayfasındaki [`OleObject`](../../../aspose.cells.drawing/oleobject/) koleksiyonunu temsil eder.

```csharp
public OleObjectCollection OleObjects { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyOleObjectsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir OleObject ekle
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, File.ReadAllBytes(@"C:\temp\example.xlsx"));
            OleObject ole = worksheet.OleObjects[oleObjectIndex];
            
            // OleObject özelliklerini değiştir
            ole.ObjectSourceFullName = @"C:\temp\modified.xlsx";
            ole.FileFormatType = FileFormatType.Xlsx;

            // Çalışma kitabını kaydedin
            workbook.Save(@"C:\temp\output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObjectCollection](../../../aspose.cells.drawing/oleobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


