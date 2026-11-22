---
title: "WorksheetCollection.BuiltInDocumentProperties"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorksheetCollection. تُرجع مجموعة DocumentProperty التي تمثل جميع خصائص المستند المدمجة في جدول البيانات"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/builtindocumentproperties/
---
## WorksheetCollection.BuiltInDocumentProperties property

تُرجع مجموعة [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) التي تمثل جميع خصائص المستند المدمجة في جدول البيانات.

```csharp
public BuiltInDocumentPropertyCollection BuiltInDocumentProperties { get; }
```

### ملاحظات

لا يمكن إضافة خاصية جديدة إلى قائمة خصائص المستند المدمجة. يمكنك فقط الحصول على خاصية مدمجة وتغيير قيمتها. القائمة التالية هي أسماء الخصائص المدمجة:

العنوان

الموضوع

المؤلف

الكلمات المفتاحية

التعليقات

القالب

المؤلف الأخير

رقم المراجعة

اسم التطبيق

تاريخ الطباعة الأخير

تاريخ الإنشاء

وقت الحفظ الأخير

إجمالي وقت التحرير

عدد الصفحات

عدد الكلمات

عدد الأحرف

الأمان

الفئة

التنسيق

المدير

الشركة

عدد البايتات

عدد الأسطر

عدد الفقرات

عدد الشرائح

عدد الملاحظات

عدد الشرائح المخفية

عدد مقاطع الوسائط المتعددة

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyBuiltInDocumentPropertiesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            DocumentProperty authorProperty = workbook.Worksheets.BuiltInDocumentProperties["Author"];
            authorProperty.Value = "John Smith";
            
            DocumentProperty titleProperty = workbook.Worksheets.BuiltInDocumentProperties["Title"];
            titleProperty.Value = "Sample Document";
            
            Console.WriteLine("Document properties set successfully");
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


