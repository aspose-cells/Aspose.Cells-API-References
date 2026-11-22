---
title: "TableStyleElement.Size"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TableStyleElement. عدد الصفوف أو الأعمدة في شريط واحد من التخطيط. تُطبق فقط عندما يكون النوع firstRowStripe أو secondRowStripe أو firstColumnStripe أو secondColumnStripe"
type: docs
url: /ar/net/aspose.cells.tables/tablestyleelement/size/
---
## TableStyleElement.Size property

عدد الصفوف أو الأعمدة في شريط واحد من التخطيط. ينطبق فقط عندما يكون النوع firstRowStripe أو secondRowStripe أو firstColumnStripe أو secondColumnStripe.

```csharp
public int Size { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementPropertySizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة لإنشاء جدول
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // إنشاء جدول
            int tableIndex = worksheet.ListObjects.Add(0, 0, 9, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // إنشاء نمط جدول باستخدام مجموعة الأنماط في المصنف
            TableStyleCollection styleCollection = workbook.Worksheets.TableStyles;
            int styleIndex = styleCollection.AddTableStyle("CustomStyle");
            TableStyle style = styleCollection[styleIndex];
            table.TableStyleName = style.Name;

            // إضافة عناصر الشرائط لتوضيح خاصية Size
            style.TableStyleElements.Add(TableStyleElementType.FirstRowStripe);
            style.TableStyleElements.Add(TableStyleElementType.SecondRowStripe);

            // الوصول إلى عناصر الشرائط
            TableStyleElement firstStripe = style.TableStyleElements[TableStyleElementType.FirstRowStripe];
            TableStyleElement secondStripe = style.TableStyleElements[TableStyleElementType.SecondRowStripe];

            // عرض قيم Size الحالية
            Console.WriteLine("Initial First Stripe Size: " + firstStripe.Size);
            Console.WriteLine("Initial Second Stripe Size: " + secondStripe.Size);

            // تعديل أحجام الشرائط
            firstStripe.Size = 2;
            secondStripe.Size = 3;

            // عرض القيم المعدلة
            Console.WriteLine("Modified First Stripe Size: " + firstStripe.Size);
            Console.WriteLine("Modified Second Stripe Size: " + secondStripe.Size);

            // حفظ المصنف لرؤية التأثيرات
            workbook.Save("TableStyleElementSizeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


