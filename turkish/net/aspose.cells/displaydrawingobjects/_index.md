---
title: "Enum DisplayDrawingObjects"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DisplayDrawingObjects enum. Çalışma kitabındaki nesnelerin gösterilip gösterilmeyeceğini ve nasıl gösterileceğini temsil eder."
type: docs
url: /tr/net/aspose.cells/displaydrawingobjects/
---
## DisplayDrawingObjects enumeration

Çalışma kitabında nesnelerin gösterilip gösterilmeyeceğini ve nasıl gösterileceğini temsil eder.

```csharp
public enum DisplayDrawingObjects
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| DisplayShapes | `0` | Tüm nesneleri göster |
| Placeholders | `1` | Yer tutucuları göster |
| Hide | `2` | Tüm şekilleri gizle. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DisplayDrawingObjectsDemo
    {
        public static void DisplayDrawingObjectsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabı ayarlarına erişin
            WorkbookSettings settings = workbook.Settings;

            // DisplayDrawingObjects özelliğini tüm nesneleri gösterecek şekilde ayarla
            settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;

            // Çalışma kitabını kaydedin
            workbook.Save("DisplayDrawingObjectsExample_DisplayShapes.xlsx");

            // DisplayDrawingObjects özelliğini yer tutucuları gösterecek şekilde ayarla
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Placeholders;

            // Çalışma kitabını kaydedin
            workbook.Save("DisplayDrawingObjectsExample_Placeholders.xlsx");

            // DisplayDrawingObjects özelliğini tüm şekilleri gizleyecek şekilde ayarla
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Hide;

            // Çalışma kitabını kaydedin
            workbook.Save("DisplayDrawingObjectsExample_Hide.xlsx");
            workbook.Save("DisplayDrawingObjectsExample_Hide.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


