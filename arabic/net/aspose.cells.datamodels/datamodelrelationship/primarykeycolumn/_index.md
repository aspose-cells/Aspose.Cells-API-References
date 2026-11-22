---
title: "DataModelRelationship.PrimaryKeyColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataModelRelationship. تحصل على اسم عمود جدول المفتاح الأساسي لهذا الارتباط"
type: docs
url: /ar/net/aspose.cells.datamodels/datamodelrelationship/primarykeycolumn/
---
## DataModelRelationship.PrimaryKeyColumn property

يحصل على اسم عمود جدول المفتاح الأساسي لهذه العلاقة.

```csharp
public string PrimaryKeyColumn { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelRelationshipPropertyPrimaryKeyColumnDemo
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
                    // عرض قيمة خاصية PrimaryKeyColumn (للقراءة فقط)
                    Console.WriteLine("Primary Key Column: " + relationship.PrimaryKeyColumn);
                }
                else
                {
                    Console.WriteLine("No relationships found in the data model.");
                }

                // احفظ المصنف
                workbook.Save("PrimaryKeyColumnDemo.xlsx");
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


