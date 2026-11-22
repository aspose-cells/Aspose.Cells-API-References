---
title: "WorkbookSettings.UpdateAdjacentCellsBorder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تشير إلى ما إذا كان يتم تحديث حدود الخلايا المجاورة"
type: docs
url: /ar/net/aspose.cells/workbooksettings/updateadjacentcellsborder/
---
## WorkbookSettings.UpdateAdjacentCellsBorder property

يشير إلى ما إذا كان يتم تحديث حد الخلايا المجاورة.

```csharp
public bool UpdateAdjacentCellsBorder { get; set; }
```

### ملاحظات

القيمة الافتراضية هي false. على سبيل المثال: الحد السفلي للخلية A1 يتم تحديثه، يجب أيضًا تغيير الحد العلوي للخلية A2.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyUpdateAdjacentCellsBorderDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // تمكين تحديث حدود الخلايا المجاورة
            workbook.Settings.UpdateAdjacentCellsBorder = true;

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين القيمة وتطبيق الحد على الخلية A1
            worksheet.Cells["A1"].PutValue("Sample");
            Style styleA1 = workbook.CreateStyle();
            styleA1.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            styleA1.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            worksheet.Cells["A1"].SetStyle(styleA1);

            // تعيين القيمة للخلية المجاورة B1 (يمين A1)
            worksheet.Cells["B1"].PutValue("Adjacent");

            // احفظ المصنف
            workbook.Save("output.xlsx");

            Console.WriteLine("Workbook saved with adjacent cell border update enabled.");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


