---
title: "TableStyleElement.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TableStyleElement. يحصل على نوع العنصر"
type: docs
url: /ar/net/aspose.cells.tables/tablestyleelement/type/
---
## TableStyleElement.Type property

يحصل على نوع العنصر.

```csharp
public TableStyleElementType Type { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة لإنشاء جدول
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // إنشاء جدول
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // احصل على نمط الجدول (باستخدام اسم النمط بدلاً من إنشاء واحد جديد)
            string styleName = table.TableStyleName;
            TableStyle style = workbook.Worksheets.TableStyles[styleName];

            // الوصول إلى عناصر نمط الجدول
            TableStyleElement element = style.TableStyleElements[TableStyleElementType.HeaderRow];

            // اعرض النوع الحالي للعنصر
            Console.WriteLine("Current Type value: " + element.Type);

            // ملاحظة: خاصية Type للقراءة فقط، لذا لا يمكننا تعيينها
            // element.Type = TableStyleElementType.TotalRow; // سيؤدي هذا إلى خطأ في التجميع

            // أظهر كيف تؤثر أنواع العناصر المختلفة على الجدول
            Console.WriteLine("\nAvailable table style elements:");
            foreach (TableStyleElementType type in Enum.GetValues(typeof(TableStyleElementType)))
            {
                try
                {
                    TableStyleElement testElement = style.TableStyleElements[type];
                    Console.WriteLine($"Element type {type} exists in this style");
                }
                catch
                {
                    Console.WriteLine($"Element type {type} not available in this style");
                }
            }

            // احفظ المصنف
            workbook.Save("TableStyleElementTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TableStyleElementType](../../tablestyleelementtype/)
* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


