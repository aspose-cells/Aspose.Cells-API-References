---
title: "الفئة DataModelRelationship"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.DataModels.DataModelRelationship. تمثل علاقة واحدة في نموذج بيانات جدول البيانات"
type: docs
url: /ar/net/aspose.cells.datamodels/datamodelrelationship/
---
## DataModelRelationship class

يمثل علاقة واحدة في نموذج بيانات جدول البيانات.

```csharp
public class DataModelRelationship
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ForeignKeyColumn](../../aspose.cells.datamodels/datamodelrelationship/foreignkeycolumn/) { get; } | يحصل على اسم عمود جدول المفتاح الأجنبي لهذه العلاقة. |
| [ForeignKeyTable](../../aspose.cells.datamodels/datamodelrelationship/foreignkeytable/) { get; } | يحصل على اسم جدول المفتاح الأجنبي لهذه العلاقة. |
| [PrimaryKeyColumn](../../aspose.cells.datamodels/datamodelrelationship/primarykeycolumn/) { get; } | يحصل على اسم عمود جدول المفتاح الأساسي لهذه العلاقة. |
| [PrimaryKeyTable](../../aspose.cells.datamodels/datamodelrelationship/primarykeytable/) { get; } | يحصل على اسم جدول المفتاح الأساسي لهذه العلاقة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelsClassDataModelRelationshipDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة للعرض
            worksheet.Cells["A1"].PutValue("Orders");
            worksheet.Cells["A2"].PutValue("OrderID");
            worksheet.Cells["A3"].PutValue("CustomerID");
            worksheet.Cells["A4"].PutValue("OrderDate");
            
            worksheet.Cells["C1"].PutValue("Customers");
            worksheet.Cells["C2"].PutValue("CustomerID");
            worksheet.Cells["C3"].PutValue("CustomerName");
            worksheet.Cells["C4"].PutValue("ContactName");

            // هذا يوضح الوصول إلى خصائص علاقة موجودة
            // في سيناريو حقيقي، ستحصل على هذا من نموذج البيانات
            DataModelRelationship relationship = workbook.DataModel?.Relationships?[0];
            if (relationship != null)
            {
                // عرض خصائص العلاقة (للقراءة فقط)
                Console.WriteLine("Sample Data Model Relationship Properties:");
                Console.WriteLine("Primary Key Table: " + relationship.PrimaryKeyTable);
                Console.WriteLine("Primary Key Column: " + relationship.PrimaryKeyColumn);
                Console.WriteLine("Foreign Key Table: " + relationship.ForeignKeyTable);
                Console.WriteLine("Foreign Key Column: " + relationship.ForeignKeyColumn);
            }
            else
            {
                Console.WriteLine("No data model relationships found");
            }

            // احفظ المصنف
            workbook.Save("DataModelRelationshipDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


