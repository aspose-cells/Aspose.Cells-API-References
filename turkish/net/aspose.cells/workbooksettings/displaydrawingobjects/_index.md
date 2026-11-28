---
title: "WorkbookSettings.DisplayDrawingObjects"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Çalışma kitabındaki nesnelerin gösterilip gösterilmeyeceğini ve nasıl gösterileceğini belirtir"
type: docs
url: /tr/net/aspose.cells/workbooksettings/displaydrawingobjects/
---
## WorkbookSettings.DisplayDrawingObjects property

Çalışma kitabındaki nesnelerin gösterilip gösterilmeyeceğini ve nasıl gösterileceğini gösterir.

```csharp
public DisplayDrawingObjects DisplayDrawingObjects { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDisplayDrawingObjectsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabı ayarlarına erişin
            WorkbookSettings settings = workbook.Settings;

            // Özelliği göstermek için örnek bir şekil ekle
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Tüm şekilleri gösterecek şekilde ayarla
            settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;
            workbook.Save("DisplayShapes.xlsx");

            // Yer tutucuları gösterecek şekilde ayarla
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Placeholders;
            workbook.Save("Placeholders.xlsx");

            // Tüm şekilleri gizleyecek şekilde ayarla
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Hide;
            workbook.Save("Hide.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [DisplayDrawingObjects](../../displaydrawingobjects/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


