---
title: "DataSorter.AddColorKey"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة DataSorter. يضيف مفتاح فرز لوني"
type: docs
url: /ar/net/aspose.cells/datasorter/addcolorkey/
---
## DataSorter.AddColorKey method

يضيف مفتاح فرز اللون.

```csharp
public void AddColorKey(int key, SortOnType type, SortOrder order, Color color)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| مفتاح | Int32 | فهرس العمود المرتب (الموضع المطلق، العمود A هو 0، B هو 1، ...) |
| type | SortOnType | نوع قيمة اللون المرتبة. |
| ترتيب | SortOrder | ترتيب الفرز. |
| اللون | اللون | لون الفرز المخصص. |

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddColorKeyWithInt32SortOnTypeSortOrderColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة مع خلايا ملونة
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue(5);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(7);
            
            // تطبيق الألوان على الخلايا
            Style styleRed = workbook.CreateStyle();
            styleRed.ForegroundColor = Color.Red;
            styleRed.Pattern = BackgroundType.Solid;
            worksheet.Cells["A2"].SetStyle(styleRed);
            
            Style styleBlue = workbook.CreateStyle();
            styleBlue.ForegroundColor = Color.Blue;
            styleBlue.Pattern = BackgroundType.Solid;
            worksheet.Cells["A3"].SetStyle(styleBlue);
            
            Style styleGreen = workbook.CreateStyle();
            styleGreen.ForegroundColor = Color.Green;
            styleGreen.Pattern = BackgroundType.Solid;
            worksheet.Cells["A4"].SetStyle(styleGreen);

            // أنشئ مُرتب البيانات وأضف مفتاح اللون
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;
            sorter.AddColorKey(0, SortOnType.CellColor, SortOrder.Ascending, Color.Red);

            // فرز البيانات
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A4"));

            // أخرج القيم المرتبة (للتوضيح)
            Console.WriteLine("Sorted values:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + (i + 1)].IntValue);
            }
        }
    }
}
```

### انظر أيضًا

* enum [SortOnType](../../sortontype/)
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


