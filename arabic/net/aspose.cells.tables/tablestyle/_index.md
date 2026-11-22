---
title: "الفئة TableStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Tables.TableStyle. تمثل نمط الجدول"
type: docs
url: /ar/net/aspose.cells.tables/tablestyle/
---
## TableStyle class

يمثل نمط الجدول.

```csharp
public class TableStyle
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Name](../../aspose.cells.tables/tablestyle/name/) { get; } | يحصل على اسم نمط الجدول. |
| [TableStyleElements](../../aspose.cells.tables/tablestyle/tablestyleelements/) { get; } | يحصل على جميع عناصر نمط الجدول. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [Create](../../aspose.cells.tables/tablestyle/create/)(string, WorksheetCollection) | ينشئ نمط جدول/جدول محوري فارغ. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleDemo
    {
        public static void TableStyleExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إنشاء أنماط للعمودين الأول والأخير
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            Style lastColumnStyle = workbook.CreateStyle();
            lastColumnStyle.Font.IsBold = true;
            lastColumnStyle.Pattern = BackgroundType.Solid;
            lastColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            // تحديد اسم نمط جدول مخصص
            string tableStyleName = "Custom1";

            // الوصول إلى مجموعة أنماط الجدول
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            // إضافة نمط جدول جديد إلى المجموعة
            int index1 = tableStyles.AddTableStyle(tableStyleName);
            TableStyle tableStyle = tableStyles[index1];

            // الوصول إلى مجموعة عناصر نمط الجدول
            TableStyleElementCollection elements = tableStyle.TableStyleElements;

            // إضافة وتعيين النمط للعمود الأول
            index1 = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[index1];
            element.SetElementStyle(firstColumnStyle);

            // إضافة وتعيين النمط للعمود الأخير
            index1 = elements.Add(TableStyleElementType.LastColumn);
            element = elements[index1];
            element.SetElementStyle(lastColumnStyle);

            // الوصول إلى خلايا ورقة العمل الأولى
            Cells cells = workbook.Worksheets[0].Cells;

            // ملء الصف الأول بأسماء الأعمدة
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }

            // ملء باقي الخلايا ببيانات عينة
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // إضافة جدول إلى ورقة العمل
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // تطبيق نمط الجدول المخصص على الجدول
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.TableStyleName = tableStyleName;

            // احفظ المصنف
            workbook.Save("TableStyleExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


