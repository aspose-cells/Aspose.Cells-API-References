---
title: "ListObject.ShowTableStyleRowStripes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListObject. تشير إلى ما إذا كان تنسيق خطوط الصفوف المرقّطة مطبقًا على"
type: docs
url: /ar/net/aspose.cells.tables/listobject/showtablestylerowstripes/
---
## ListObject.ShowTableStyleRowStripes property

يشير إلى ما إذا كان تنسيق الشرائط الصفية مطبقًا.

```csharp
public bool ShowTableStyleRowStripes { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTableStyleRowStripesDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("Item3");
            worksheet.Cells["B4"].PutValue(300);

            // إنشاء كائن قائمة
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add("A1", "B4", true);
            ListObject listObject = listObjects[index];

            // عرض خاصية ShowTableStyleRowStripes
            Console.WriteLine("Before: ShowTableStyleRowStripes = " + listObject.ShowTableStyleRowStripes);
            listObject.ShowTableStyleRowStripes = false;
            Console.WriteLine("After: ShowTableStyleRowStripes = " + listObject.ShowTableStyleRowStripes);

            // احفظ المصنف
            workbook.Save("ListObjectShowTableStyleRowStripesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


