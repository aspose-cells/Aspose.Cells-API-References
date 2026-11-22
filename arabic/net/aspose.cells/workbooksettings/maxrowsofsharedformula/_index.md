---
title: "WorkbookSettings.MaxRowsOfSharedFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تحصل وتعيّن الحد الأقصى لعدد الصفوف للصيغة المشتركة"
type: docs
url: /ar/net/aspose.cells/workbooksettings/maxrowsofsharedformula/
---
## WorkbookSettings.MaxRowsOfSharedFormula property

يحصل أو يضبط أقصى رقم للصف للمعادلة المشتركة.

```csharp
public int MaxRowsOfSharedFormula { get; set; }
```

### ملاحظات

إذا كان الرقم كبيرًا جدًا، يعمل الفلتر التلقائي ببطء شديد في MS Excel 2013.

### أمثلة

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
            
            // تعيين صيغة مشتركة بـ 101 صف (يتجاوز MaxRowsOfSharedFormula)
            cells["B1"].SetSharedFormula("=A1", 101, 1);
            
            // تحقق من الصيغة في الخلية الأخيرة
            Console.WriteLine("Formula in B101: " + cells["B101"].Formula);
            
            // زيادة MaxRowsOfSharedFormula واختبار مرة أخرى في ورقة جديدة
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

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


