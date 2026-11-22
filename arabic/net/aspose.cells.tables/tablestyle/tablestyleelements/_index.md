---
title: "TableStyle.TableStyleElements"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TableStyle. تحصل على جميع عناصر نمط الجدول"
type: docs
url: /ar/net/aspose.cells.tables/tablestyle/tablestyleelements/
---
## TableStyle.TableStyleElements property

يحصل على جميع عناصر نمط الجدول.

```csharp
public TableStyleElementCollection TableStyleElements { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStylePropertyTableStyleElementsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة للجدول
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // إنشاء جدول
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTableStyleFirstColumn = true;

            // احصل على نمط الجدول (استخدم النمط الموجود بدلاً من إنشاء واحد جديد)
            TableStyle style = workbook.Worksheets.TableStyles[0];

            // تعديل عناصر نمط الجدول
            TableStyleElement wholeTableElement = style.TableStyleElements[TableStyleElementType.WholeTable];
            Style wholeTableStyle = wholeTableElement.GetElementStyle();
            wholeTableStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            wholeTableStyle.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;

            // تطبيق النمط المعدل على الجدول
            table.TableStyleName = style.Name;

            // احفظ المصنف
            workbook.Save("TableStyleElementsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TableStyleElementCollection](../../tablestyleelementcollection/)
* class [TableStyle](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


