---
title: "WorkbookSettings.MaxRowsOfSharedFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Paylaşılan formülün maksimum satır sayısını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/workbooksettings/maxrowsofsharedformula/
---
## WorkbookSettings.MaxRowsOfSharedFormula property

Paylaşılan formülün maksimum satır sayısını alır ve ayarlar.

```csharp
public int MaxRowsOfSharedFormula { get; set; }
```

### Açıklamalar

Sayı çok büyükse, otomatik filtre MS Excel 2013'te çok yavaş çalışır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMaxRowsOfSharedFormulaDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            book.Settings.MaxRowsOfSharedFormula = 100;
            
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // 101 satırla ortak formül ayarla (MaxRowsOfSharedFormula değerini aşıyor)
            cells["B1"].SetSharedFormula("=A1", 101, 1);
            
            // Son hücredeki formülü doğrula
            Console.WriteLine("Formula in B101: " + cells["B101"].Formula);
            
            // MaxRowsOfSharedFormula değerini artır ve yeni sayfada tekrar test et
            book.Settings.MaxRowsOfSharedFormula = 1024;
            Worksheet sheet2 = book.Worksheets.Add("Sheet2");
            cells = sheet2.Cells;
            cells["B1"].SetSharedFormula("=A1", 101, 1);
            
            Console.WriteLine("Formula in B101 (Sheet2): " + cells["B101"].Formula);
            
            book.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


