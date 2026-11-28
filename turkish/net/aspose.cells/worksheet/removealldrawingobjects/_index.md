---
title: "Worksheet.RemoveAllDrawingObjects"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Bu çalışma sayfasındaki tüm çizim nesnelerini kaldırır"
type: docs
url: /tr/net/aspose.cells/worksheet/removealldrawingobjects/
---
## Worksheet.RemoveAllDrawingObjects method

Bu çalışma sayfasındaki tüm çizim nesnelerini kaldırır.

```csharp
public void RemoveAllDrawingObjects()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRemoveAllDrawingObjectsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bazı çizim nesneleri ekle
            worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 50);
            worksheet.Shapes.AddLine(1, 0, 5, 100, 5, 150);
            
            // Nesneleri kaldırmadan önce kaydet
            workbook.Save("BeforeRemove.xlsx", SaveFormat.Xlsx);
            
            // Tüm çizim nesnelerini kaldır
            worksheet.RemoveAllDrawingObjects();
            
            // Nesneleri kaldırdıktan sonra kaydet
            workbook.Save("AfterRemove.xlsx", SaveFormat.Xlsx);
            
            // Çalışma kitabını serbest bırak
            workbook.Dispose();
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


