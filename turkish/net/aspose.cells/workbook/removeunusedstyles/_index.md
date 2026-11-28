---
title: "Workbook.RemoveUnusedStyles"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Kullanılmayan tüm stilleri kaldır"
type: docs
url: /tr/net/aspose.cells/workbook/removeunusedstyles/
---
## Workbook.RemoveUnusedStyles method

Kullanılmayan tüm stilleri kaldır.

```csharp
public void RemoveUnusedStyles()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveUnusedStylesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = wb.Worksheets[0];
            
            // Stillerle bazı örnek veriler ekle
            for (int i = 0; i < 10; i++)
            {
                Cell cell = sheet.Cells[i, 0];
                cell.PutValue("Item " + (i + 1));
                
                // Hücrelere farklı stiller uygula
                Style style = wb.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 10 + i;
                style.Font.IsBold = i % 2 == 0;
                cell.SetStyle(style);
            }
            
            // Kullanılmayan stilleri bırakmak için bazı hücreleri kaldır
            sheet.Cells.DeleteRows(5, 5);
            
            // Kullanılmayan stilleri kaldırmadan önce kaydet
            wb.Save("BeforeRemoveUnusedStyles.xlsx");
            
            // Kullanılmayan stilleri kaldır
            wb.RemoveUnusedStyles();
            
            // Kullanılmayan stilleri kaldırdıktan sonra kaydet
            wb.Save("AfterRemoveUnusedStyles.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


