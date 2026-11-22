---
title: "الفئة DataModel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.DataModels.DataModel. تمثل نموذج البيانات"
type: docs
url: /ar/net/aspose.cells.datamodels/datamodel/
---
## DataModel class

يمثل نموذج البيانات.

```csharp
public class DataModel
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Relationships](../../aspose.cells.datamodels/datamodel/relationships/) { get; } | يحصل على جميع العلاقات بين الجداول في نموذج البيانات. |
| [Tables](../../aspose.cells.datamodels/datamodel/tables/) { get; } | يحصل على جميع الجداول في نموذج البيانات. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelsClassDataModelDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // احصل على DataModel من المصنف بدلاً من إنشاء نسخة جديدة
            DataModel dataModel = workbook.DataModel;

            // إظهار الوصول إلى الجداول والعلاقات (خصائص للقراءة فقط)
            Console.WriteLine("Number of tables in DataModel: " + dataModel.Tables.Count);
            Console.WriteLine("Number of relationships in DataModel: " + dataModel.Relationships.Count);

            // ملاحظة: نظرًا لأن الجداول والعلاقات هي مجموعات للقراءة فقط،
            // يمكننا فقط الوصول إلى العناصر الموجودة ولكن لا يمكن تعديلها مباشرة

            // حفظ المصنف (عادةً ما يُستخدم DataModel داخليًا بواسطة Aspose.Cells)
            workbook.Save("DataModelDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


