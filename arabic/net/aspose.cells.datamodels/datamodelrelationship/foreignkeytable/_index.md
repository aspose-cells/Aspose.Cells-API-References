---
title: "DataModelRelationship.ForeignKeyTable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataModelRelationship. تحصل على اسم جدول المفتاح الأجنبي لهذا الارتباط"
type: docs
url: /ar/net/aspose.cells.datamodels/datamodelrelationship/foreignkeytable/
---
## DataModelRelationship.ForeignKeyTable property

يحصل على اسم جدول المفتاح الأجنبي لهذه العلاقة.

```csharp
public string ForeignKeyTable { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelRelationshipPropertyForeignKeyTableDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات تجريبية لإنشاء سياق ذو معنى
            worksheet.Cells["A1"].PutValue("Orders");
            worksheet.Cells["A2"].PutValue("OrderID");
            worksheet.Cells["A3"].PutValue("CustomerID");

            worksheet.Cells["C1"].PutValue("Customers");
            worksheet.Cells["C2"].PutValue("CustomerID");
            worksheet.Cells["C3"].PutValue("CustomerName");

            try
            {
                // الوصول إلى أول ارتباط إذا كان موجودًا
                DataModelRelationship relationship = workbook.DataModel?.Relationships?[0];

                if (relationship != null)
                {
                    // عرض قيمة خاصية ForeignKeyTable (للقراءة فقط)
                    Console.WriteLine("Foreign Key Table: " + relationship.ForeignKeyTable);
                }
                else
                {
                    Console.WriteLine("No relationships found in the data model.");
                }

                // احفظ المصنف
                workbook.Save("ForeignKeyTableDemo.xlsx");
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

* class [DataModelRelationship](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


