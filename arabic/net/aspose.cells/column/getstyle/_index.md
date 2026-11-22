---
title: "Column.GetStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Column. تحصل على نمط هذا العمود"
type: docs
url: /ar/net/aspose.cells/column/getstyle/
---
## Column.GetStyle method

يحصل على نمط هذا العمود.

```csharp
public Style GetStyle()
```

### ملاحظات

تعديل كائن النمط المرتجع مباشرة لا يؤثر على هذا العمود أو أي خلايا في هذا العمود. عليك استدعاء طريقة [`ApplyStyle`](../applystyle/) أو طريقة [`SetStyle`](../setstyle/) لتطبيق التغيير على هذا العمود. نمط العمود هو النمط الذي سيُورث إلى الخلايا في هذا العمود (تلك الخلايا التي لا تحتوي على إعدادات نمط مخصصة، مثل الخلايا الموجودة التي لم يتم تعيين نمط لها صراحةً، أو تلك التي لم يتم إنشاءها).

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnMethodGetStyleDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // عيّن النمط للعمود 5
            Style columnStyle = cells.Columns[5].GetStyle();
            columnStyle.Font.Name = "Arial";
            columnStyle.Font.Size = 14;
            columnStyle.Font.IsBold = true;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { Font = true });

            // تعيين نمط للصف 7
            Style rowStyle = cells.Rows[7].GetStyle();
            rowStyle.Font.Color = System.Drawing.Color.Red;
            rowStyle.Font.IsItalic = true;
            cells.Rows[7].ApplyStyle(rowStyle, new StyleFlag { Font = true });

            // تحقق من نمط العمود
            Style retrievedColumnStyle = cells.Columns[5].GetStyle();
            Console.WriteLine("Column 5 Style:");
            Console.WriteLine($"Font: {retrievedColumnStyle.Font.Name}, Size: {retrievedColumnStyle.Font.Size}, Bold: {retrievedColumnStyle.Font.IsBold}");

            // تحقق من نمط الصف
            Style retrievedRowStyle = cells.Rows[7].GetStyle();
            Console.WriteLine("\nRow 7 Style:");
            Console.WriteLine($"Color: {retrievedRowStyle.Font.Color}, Italic: {retrievedRowStyle.Font.IsItalic}");

            // احفظ المصنف
            workbook.Save("ColumnMethodGetStyleDemo_output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


