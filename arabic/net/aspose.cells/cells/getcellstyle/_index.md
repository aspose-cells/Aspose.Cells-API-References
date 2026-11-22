---
title: "Cells.GetCellStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. احصل على نمط الخلية المعطاة"
type: docs
url: /ar/net/aspose.cells/cells/getcellstyle/
---
## Cells.GetCellStyle method

احصل على نمط الخلية المعطاة.

```csharp
public Style GetCellStyle(int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف |
| عمود | Int32 | عمود |

### قيمة الإرجاع

نمط الخلية المعطاة.

### ملاحظات

النمط المرتجع هو فقط النمط المحدد للخلية أو الموروث من الصف/العمود الخاص بالخلية، ولا يتضمن الخصائص المطبقة بواسطة إعدادات أخرى مثل التنسيقات الشرطية.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsMethodGetCellStyleWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى الخلية B5 (الصف 4، العمود 1) وتعيين النمط الأولي
            Cell cell = worksheet.Cells["B5"];
            cell.PutValue("Styled Cell");
            
            // إنشاء وتطبيق النمط الأولي للخلية
            Style initialStyle = workbook.CreateStyle();
            initialStyle.Font.IsBold = true;  // Changed from Bold to IsBold
            initialStyle.BackgroundColor = Color.LightYellow;
            cell.SetStyle(initialStyle);

            try
            {
                // استدعِ GetCellStyle مع معلمات Int32 (الصف 4، العمود 1)
                Style cellStyle = worksheet.Cells.GetCellStyle(4, 1);

                // اعرض خصائص النمط المسترجع
                Console.WriteLine($"Retrieved style - Bold: {cellStyle.Font.IsBold}, Background: {cellStyle.BackgroundColor}");  // Changed from Bold to IsBold

                // عدّل النمط المسترجع
                cellStyle.Font.IsItalic = true;  // Changed from Italic to IsItalic
                cellStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

                // طبق النمط المعدل مرة أخرى على الخلية
                cell.SetStyle(cellStyle);

                Console.WriteLine("GetCellStyle executed successfully. Modified border and font style.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellStyle: {ex.Message}");
            }

            // احفظ المصنف المعدل
            workbook.Save("CellsGetCellStyleWithInt32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


