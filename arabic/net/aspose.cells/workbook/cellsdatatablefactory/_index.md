---
title: "Workbook.CellsDataTableFactory"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تحصل على المصنع لإنشاء ICellsDataTable من الكائنات المخصصة"
type: docs
url: /ar/net/aspose.cells/workbook/cellsdatatablefactory/
---
## Workbook.CellsDataTableFactory property

يحصل على المصنع لبناء ICellsDataTable من الكائنات المخصصة

```csharp
public CellsDataTableFactory CellsDataTableFactory { get; }
```

### أمثلة

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomData
    {
        public int Id { get; set; }
        public string Name { get; set; }
        public int Age { get; set; }
    }

    public class WorkbookPropertyCellsDataTableFactoryDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            List<CustomData> dataList = new List<CustomData>
            {
                new CustomData { Id = 1, Name = "John Doe", Age = 30 },
                new CustomData { Id = 2, Name = "Jane Smith", Age = 25 },
                new CustomData { Id = 3, Name = "Sam Brown", Age = 35 }
            };

            // الحصول على CellsDataTableFactory من خاصية workbook
            CellsDataTableFactory factory = workbook.CellsDataTableFactory;

            // إنشاء جدول بيانات من قائمة
            ICellsDataTable dataTable = factory.GetInstance(dataList);

            // استيراد البيانات إلى ورقة العمل
            sheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

            // احفظ المخرجات
            workbook.Save("CellsDataTableFactoryDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CellsDataTableFactory](../../cellsdatatablefactory/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


