---
title: "WorkbookSettings.MaxColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Sıfır tabanlı en yüksek sütun indeksini alır"
type: docs
url: /tr/net/aspose.cells/workbooksettings/maxcolumn/
---
## WorkbookSettings.MaxColumn property

Sıfır tabanlı maksimum sütun dizinini alır.

```csharp
public int MaxColumn { get; }
```

### Açıklamalar

Dosya formatı Excel97-2003 ise 255 döndürür;

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMaxColumnDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Console.WriteLine("MaxColumn value: " + workbook.Settings.MaxColumn);
            
            // Sınırın ötesindeki bir sütuna erişmeye çalışarak MaxColumn kullanımını gösterin
            try
            {
                Cells cells = workbook.Worksheets[0].Cells;
                Cell cell = cells[0, workbook.Settings.MaxColumn + 1];
                Console.WriteLine("This should not be reached");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Expected error when accessing beyond MaxColumn: " + ex.Message);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


