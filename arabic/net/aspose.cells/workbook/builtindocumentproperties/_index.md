---
title: "Workbook.BuiltInDocumentProperties"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تُرجع مجموعة DocumentProperty التي تمثل جميع خصائص المستند المدمجة لجدول البيانات"
type: docs
url: /ar/net/aspose.cells/workbook/builtindocumentproperties/
---
## Workbook.BuiltInDocumentProperties property

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
    public class WorkbookPropertyBuiltInDocumentPropertiesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى خصائص المستند المدمجة وتعديلها
            DocumentProperty authorProperty = workbook.BuiltInDocumentProperties["Author"];
            authorProperty.Value = "John Smith";
            
            DocumentProperty titleProperty = workbook.BuiltInDocumentProperties["Title"];
            titleProperty.Value = "Sample Workbook";
            
            // عرض الخصائص المعدلة
            Console.WriteLine("Author: " + workbook.BuiltInDocumentProperties["Author"].Value);
            Console.WriteLine("Title: " + workbook.BuiltInDocumentProperties["Title"].Value);
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


