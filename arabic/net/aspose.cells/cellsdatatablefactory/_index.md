---
title: "الفئة CellsDataTableFactory"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.CellsDataTableFactory فئة. أداة لبناء ICellsDataTable من كائنات مخصصة لتسهيل الاستخدام للمستخدمين"
type: docs
url: /ar/net/aspose.cells/cellsdatatablefactory/
---
## CellsDataTableFactory class

أداة لإنشاء ICellsDataTable من كائنات مخصصة لتسهيل الاستخدام على المستخدم.

```csharp
public class CellsDataTableFactory
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance)(double[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_6)(ICollection) | ينشئ ICellsDataTable من مجموعة مُعطاة. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_3)(int[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_8)(object[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_1)(double[], bool) | ينشئ ICellsDataTable من تسلسل القيم المزدوجة المُعطى. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_2)(double[], string[]) | ينشئ ICellsDataTable من تسلسل القيم المزدوجة المُعطى. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_7)(ICollection, bool) | ينشئ ICellsDataTable من مجموعة مُعطاة. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_4)(int[], bool) | ينشئ ICellsDataTable من تسلسل القيم الصحيحة المُعطى. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_5)(int[], string[]) | ينشئ ICellsDataTable من تسلسل القيم الصحيحة المُعطى. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_9)(object[], bool) | ينشئ ICellsDataTable من تسلسل الكائنات المُعطى. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_10)(object[], string[]) | ينشئ ICellsDataTable من تسلسل الكائنات المُعطى. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_11)(object[][], bool, string[]) | ينشئ ICellsDataTable من تسلسل الكائنات المُعطى. |

### أمثلة

```csharp
using Aspose.Cells;
using System;
using System.Collections.Generic;

namespace AsposeCellsExamples
{
    public class CellsDataTableFactoryDemo
    {
        public static void RunDemo()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            List<CustomData> dataList = new List<CustomData>
            {
                new CustomData { Id = 1, Name = "John Doe", Age = 30 },
                new CustomData { Id = 2, Name = "Jane Smith", Age = 25 },
                new CustomData { Id = 3, Name = "Sam Brown", Age = 35 }
            };

            // احصل على مثال CellsDataTableFactory من المصنف
            CellsDataTableFactory factory = workbook.CellsDataTableFactory;

            // إنشاء مثال ICellsDataTable من قائمة البيانات المخصصة
            ICellsDataTable dataTable = factory.GetInstance(dataList);

            // استيراد جدول البيانات إلى ورقة العمل بدءًا من الخلية A1
            sheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

            // احفظ المصنف
            workbook.Save("CellsDataTableFactoryDemo.xlsx");
            workbook.Save("CellsDataTableFactoryDemo.pdf");
        }
    }

    // فئة البيانات المخصصة
    public class CustomData
    {
        public int Id { get; set; }
        public string Name { get; set; }
        public int Age { get; set; }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


