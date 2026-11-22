---
title: "الفئة IconFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.IconFilter. تمثل مرشح الأيقونة"
type: docs
url: /ar/net/aspose.cells/iconfilter/
---
## IconFilter class

يمثل مرشح الأيقونات.

```csharp
public class IconFilter
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [IconId](../../aspose.cells/iconfilter/iconid/) { get; set; } | يحصل ويضبط الفهرس الصفري لرمز في مجموعة الأيقونات. |
| [IconSetType](../../aspose.cells/iconfilter/iconsettype/) { get; set; } | يحصل ويضبط مجموعة الأيقونات المستخدمة لهذا المعيار. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassIconFilterDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // ملء بيانات عينة
                for (int i = 0; i < 10; i++)
                {
                    worksheet.Cells[i, 0].PutValue(i * 10);
                }

                // إنشاء مرشح تلقائي
                worksheet.AutoFilter.Range = "A1:A10";
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
                filterColumn.FilterType = FilterType.IconFilter;

                // احصل على مرشح الأيقونة
                IconFilter iconFilter = (IconFilter)filterColumn.Filter;

                // تعيين خصائص مرشح الأيقونة
                iconFilter.IconSetType = IconSetType.Arrows3;
                iconFilter.IconId = 1; // Filter for middle arrow

                Console.WriteLine($"IconFilter created with IconSetType: {iconFilter.IconSetType} and IconId: {iconFilter.IconId}");

                // احفظ المصنف
                workbook.Save("IconFilterDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with icon filter applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with IconFilter: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


