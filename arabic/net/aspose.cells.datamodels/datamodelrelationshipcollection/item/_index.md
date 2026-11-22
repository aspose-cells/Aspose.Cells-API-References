---
title: "DataModelRelationshipCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataModelRelationshipCollection. تحصل على العلاقة"
type: docs
url: /ar/net/aspose.cells.datamodels/datamodelrelationshipcollection/item/
---
## DataModelRelationshipCollection indexer

يحصل على العلاقة.

```csharp
public DataModelRelationship this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelRelationshipCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد (نموذج بيانات فارغ)
            Workbook workbook = new Workbook();

            try
            {
                // احصل على DataModelRelationshipCollection من المصنف (قد يكون فارغًا إذا لم يكن هناك نموذج بيانات)
                DataModelRelationshipCollection relationships = workbook.DataModel?.Relationships;

                if (relationships == null)
                {
                    Console.WriteLine("The workbook does not contain a data model.");
                }
                else if (relationships.Count == 0)
                {
                    Console.WriteLine("The data model exists but contains no relationships.");
                }
                else
                {
                    // قراءة العلاقة الأولى باستخدام خاصية Item (المؤشر)
                    DataModelRelationship firstRelationship = relationships[0]; // Item property getter
                    Console.WriteLine("First relationship retrieved via Item property:");
                    Console.WriteLine(firstRelationship);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while accessing Item property: {ex.Message}");
            }

            // حفظ المصنف (اختياري، فقط لإظهار أن الشيفرة تعمل من البداية إلى النهاية)
            workbook.Save("ItemPropertyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DataModelRelationship](../../datamodelrelationship/)
* class [DataModelRelationshipCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


