---
title: "BuiltInDocumentPropertyCollection.Template"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "BuiltInDocumentPropertyCollection property. يحصل أو يضبط الاسم المعلوماتي لقالب المستند"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/template/
---
## BuiltInDocumentPropertyCollection.Template property

يحصل أو يضبط الاسم الإعلامي لقالب المستند.

```csharp
public string Template { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyTemplateDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى خصائص المستند المدمجة
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // قم بتعيين خاصية Template
            builtInProperties.Template = "Standard Template";

            // اضبط خصائص أساسية أخرى للتوضيح
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Template Property Demo";

            // احفظ المصنف
            workbook.Save("TemplatePropertyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


