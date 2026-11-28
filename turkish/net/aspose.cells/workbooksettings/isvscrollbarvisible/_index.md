---
title: "WorkbookSettings.IsVScrollBarVisible"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Oluşturulan elektronik tabloyun dikey kaydırma çubuğu içerip içermediğini belirten bir değeri alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/workbooksettings/isvscrollbarvisible/
---
## WorkbookSettings.IsVScrollBarVisible property

Oluşturulan elektronik tablonun dikey kaydırma çubuğu içerip içermeyeceğini belirten bir değeri alır veya ayarlar.

```csharp
public bool IsVScrollBarVisible { get; set; }
```

### Açıklamalar

Varsayılan değer true'tur.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsVScrollBarVisibleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabı ayarlarına eriş
            WorkbookSettings settings = workbook.Settings;
            
            // Dikey kaydırma çubuğunu gizle
            settings.IsVScrollBarVisible = false;
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Vertical scroll bar visibility set to false. Workbook saved.");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


