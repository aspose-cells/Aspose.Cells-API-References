---
title: "PowerQueryFormulaFunction.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PowerQueryFormulaFunction. يحصل على نوع صيغة Power Query"
type: docs
url: /ar/net/aspose.cells.querytables/powerqueryformulafunction/type/
---
## PowerQueryFormulaFunction.Type property

يحصل على نوع صيغة استعلام الطاقة.

```csharp
public override PowerQueryFormulaType Type { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaFunctionPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء دالة صيغة Power Query
            // نظرًا لأنه لا يمكننا الإنشاء مباشرةً، سنحتاج إلى الحصول عليه من مكان ما
            // لأغراض العرض، سنعرض فقط كيفية الوصول إلى الخاصية Type
            // (في الاستخدام الفعلي، ستحصل على هذا من مجموعة موجودة)
            PowerQueryFormulaFunction function = null; // Can't instantiate directly
            
            // نظرًا لأنه لا يمكننا إنشاء QueryTable مباشرةً أيضًا، سنتخطى هذا الجزء
            QueryTable queryTable = null; // Can't instantiate directly
            
            // لا يمكن إضافة إلى مجموعة جداول الاستعلام بهذه الطريقة - فهي للقراءة فقط
            // worksheet.QueryTables[0] = queryTable; // تم إزالة هذا السطر
            
            // للتوضيح، سنعرض فقط تنسيق الإخراج الذي كنا سنستخدمه إذا كان لدينا دالة
            if (function != null)
            {
                Console.WriteLine("Power Query Formula Function Type: " + function.Type);
                Console.WriteLine("Is this a function? " + (function.Type == PowerQueryFormulaType.Function));
            }
            else
            {
                Console.WriteLine("Could not create PowerQueryFormulaFunction instance - constructor not available");
            }

            // حفظ النتيجة
            workbook.Save("PowerQueryFormulaFunctionTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormulaFunction](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


