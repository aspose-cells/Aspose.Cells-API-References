---
title: "TableStyleElement.GetElementStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة TableStyleElement. يحصل على نمط العنصر"
type: docs
url: /ar/net/aspose.cells.tables/tablestyleelement/getelementstyle/
---
## TableStyleElement.GetElementStyle method

يحصل على نمط العنصر.

```csharp
public Style GetElementStyle()
```

### قيمة الإرجاع

يرجع كائن [`Style`](../../../aspose.cells/style/) .

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleElementMethodGetElementStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            
            // إنشاء جدول
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            
            // احصل على نمط الجدول من مجموعة أنماط الجدول في المصنف
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            TableStyle style = tableStyles[0];
            table.TableStyleName = style.Name;
            
            // الوصول إلى عنصر نمط الجدول الكامل
            TableStyleElement element = style.TableStyleElements[TableStyleElementType.WholeTable];
            
            // احصل على نمط العنصر
            Style tableStyle = element.GetElementStyle();
            
            // تعديل خصائص النمط
            tableStyle.Font.Name = "Arial";
            tableStyle.Font.Size = 12;
            tableStyle.Font.IsBold = true;
            tableStyle.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            tableStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            tableStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            tableStyle.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            
            // إعادة النمط المعدل
            element.SetElementStyle(tableStyle);
            
            // احفظ المصنف
            workbook.Save("TableStyleElementDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../../aspose.cells/style/)
* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


