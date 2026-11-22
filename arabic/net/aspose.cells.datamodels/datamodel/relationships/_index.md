---
title: "DataModel.Relationships"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataModel. تحصل على جميع العلاقات للجداول في نموذج البيانات"
type: docs
url: /ar/net/aspose.cells.datamodels/datamodel/relationships/
---
## DataModel.Relationships property

يحصل على جميع العلاقات بين الجداول في نموذج البيانات.

```csharp
public DataModelRelationshipCollection Relationships { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelPropertyRelationshipsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            try
            {
                // الوصول إلى DataModel من المصنف
                DataModel dataModel = workbook.DataModel;

                // عرض القيمة الحالية لخاصية Relationships (للقراءة فقط)
                Console.WriteLine("Number of relationships in DataModel: " + dataModel.Relationships.Count);

                // التكرار عبر العلاقات إذا وجدت أي منها
                foreach (DataModelRelationship relationship in dataModel.Relationships)
                {
                    Console.WriteLine("Relationship found: " + relationship);
                }

                // احفظ المصنف
                workbook.Save("RelationshipsDemo.xlsx");
                Console.WriteLine("Relationships demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [DataModelRelationshipCollection](../../datamodelrelationshipcollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


