---
title: "DocumentProperty.Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DocumentProperty. تحصل أو تعين قيمة الخاصية"
type: docs
url: /ar/net/aspose.cells.properties/documentproperty/value/
---
## DocumentProperty.Value property

يحصل أو يعيّن قيمة الخاصية.

```csharp
public object Value { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى خصائص المستند المدمجة
            var hyperlinkBase = workbook.Worksheets.BuiltInDocumentProperties["HyperlinkBase"];
            hyperlinkBase.Value = "http://www.example.com";

            var title = workbook.Worksheets.BuiltInDocumentProperties["Title"];
            title.Value = "Sample Document Title";

            // احفظ المصنف
            workbook.Save("DocumentPropertiesDemo.xlsx");

            // اعرض القيم المحددة
            Console.WriteLine("HyperlinkBase: " + hyperlinkBase.Value);
            Console.WriteLine("Title: " + title.Value);
        }
    }
}
```

### انظر أيضًا

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


