---
title: "WorkbookSettings.MaxRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Sıfır tabanlı maksimum satır indeksini alır"
type: docs
url: /tr/net/aspose.cells/workbooksettings/maxrow/
---
## WorkbookSettings.MaxRow property

Sıfır tabanlı maksimum satır dizinini alır.

```csharp
public int MaxRow { get; }
```

### Açıklamalar

Dosya formatı Excel97-2003 ise 65535 döndürür;

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMaxRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // MaxRow özelliğini gösterin
            Console.WriteLine("Maximum rows in worksheet: " + workbook.Settings.MaxRow);
            
            // MaxRow'un ötesindeki bir hücreye erişmeye çalışın (istisna fırlatmalıdır)
            try
            {
                Cell cell = worksheet.Cells[workbook.Settings.MaxRow + 1, 0];
                Console.WriteLine("This line shouldn't execute");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Expected error when accessing beyond MaxRow: " + ex.Message);
            }
            
            // MaxRow kullanarak bir hücre alanı oluşturun
            CellArea area = CellArea.CreateCellArea(0, 0, workbook.Settings.MaxRow, 0);
            Console.WriteLine("Created cell area from row 0 to MaxRow: " + area.EndRow);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


