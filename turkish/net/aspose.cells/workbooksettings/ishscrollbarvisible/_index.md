---
title: "WorkbookSettings.IsHScrollBarVisible"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Oluşturulan elektronik tablonun bir yatay kaydırma çubuğu içerip içermediğini belirten bir değeri alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/workbooksettings/ishscrollbarvisible/
---
## WorkbookSettings.IsHScrollBarVisible property

Oluşturulan elektronik tablonun yatay kaydırma çubuğu içerip içermeyeceğini gösteren bir değeri alır veya ayarlar.

```csharp
public bool IsHScrollBarVisible { get; set; }
```

### Açıklamalar

Varsayılan değer true'tur.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsHScrollBarVisibleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabı ayarlarına eriş
            WorkbookSettings settings = workbook.Settings;
            
            // Yatay kaydırma çubuğunu gizle
            settings.IsHScrollBarVisible = false;
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with horizontal scroll bar hidden.");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


