---
title: "BuiltInDocumentPropertyCollection.HyperlinkBase"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية BuiltInDocumentPropertyCollection. تحصل أو تعين خاصية hyperlinkbase"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/hyperlinkbase/
---
## BuiltInDocumentPropertyCollection.HyperlinkBase property

يحصل أو يعيّن خاصية hyperlinkbase.

```csharp
public string HyperlinkBase { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyHyperlinkBaseDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // عيّن خاصية HyperlinkBase
            workbook.BuiltInDocumentProperties.HyperlinkBase = "http://www.example.com";

            // عيّن خاصية أخرى للتوضيح
            workbook.BuiltInDocumentProperties.Title = "Sample Workbook";

            // احفظ المصنف
            workbook.Save("HyperlinkBaseDemo.xlsx", SaveFormat.Xlsx);

            // تحميل المصنف المحفوظ للتحقق من الخصائص
            Workbook loadedWorkbook = new Workbook("HyperlinkBaseDemo.xlsx");
            
            // أخرج الخصائص إلى وحدة التحكم
            Console.WriteLine("HyperlinkBase: " + loadedWorkbook.BuiltInDocumentProperties.HyperlinkBase);
            Console.WriteLine("Title: " + loadedWorkbook.BuiltInDocumentProperties.Title);
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


