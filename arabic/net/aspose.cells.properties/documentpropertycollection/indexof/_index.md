---
title: "DocumentPropertyCollection.IndexOf"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة DocumentPropertyCollection. تحصل على فهرس خاصية حسب الاسم"
type: docs
url: /ar/net/aspose.cells.properties/documentpropertycollection/indexof/
---
## DocumentPropertyCollection.IndexOf method

يحصل على فهرس الخاصية حسب الاسم.

```csharp
public int IndexOf(string name)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم الخاصية غير حساس لحالة الأحرف. |

### قيمة الإرجاع

الفهرس الصفري. قيمة سلبية إذا لم يتم العثور عليه.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyCollectionMethodIndexOfWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // احصل على مجموعة خصائص المستند المدمجة
            DocumentPropertyCollection properties = workbook.Worksheets.BuiltInDocumentProperties;

            // بالنسبة للخصائص المدمجة، لا يمكننا إلا تعيين قيم الخصائص الموجودة
            // لإضافة خصائص مخصصة، سنحتاج إلى استخدام CustomDocumentPropertyCollection
            // هنا سنقوم فقط بتعيين بعض الخصائص المدمجة الموجودة لأغراض العرض
            properties["Title"].Value = "Value1";
            properties["Subject"].Value = "Value2";
            properties["Author"].Value = "Value3";

            try
            {
                // استدعِ طريقة IndexOf مع معامل نصي
                int index = properties.IndexOf("Subject");
                
                // اعرض النتيجة
                Console.WriteLine($"Index of 'Subject': {index}");
                
                // اعرض الخاصية في الفهرس الذي تم العثور عليه
                if (index >= 0)
                {
                    DocumentProperty property = properties[index];
                    Console.WriteLine($"Property at index {index}: {property.Name} = {property.Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IndexOf method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("DocumentPropertyIndexOfDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


