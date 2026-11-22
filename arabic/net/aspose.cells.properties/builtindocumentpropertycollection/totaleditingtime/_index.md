---
title: "BuiltInDocumentPropertyCollection.TotalEditingTime"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية BuiltInDocumentPropertyCollection. تحصل أو تضبط إجمالي وقت التحرير بالدقائق"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/totaleditingtime/
---
## BuiltInDocumentPropertyCollection.TotalEditingTime property

يحصل أو يضبط إجمالي وقت التحرير بالدقائق.

```csharp
public double TotalEditingTime { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyTotalEditingTimeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى خصائص المستند المدمجة
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // اضبط إجمالي وقت التحرير بالدقائق
            builtInProperties.TotalEditingTime = 90.5;

            // اعرض وقت التحرير المحدد
            Console.WriteLine("Total Editing Time: " + builtInProperties.TotalEditingTime + " minutes");

            // احفظ المصنف
            workbook.Save("TotalEditingTimeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


