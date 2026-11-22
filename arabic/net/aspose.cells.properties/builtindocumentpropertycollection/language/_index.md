---
title: "BuiltInDocumentPropertyCollection.Language"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية BuiltInDocumentPropertyCollection. يحصل على أو يضبط لغة المستند"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/language/
---
## BuiltInDocumentPropertyCollection.Language property

يحصل أو يضبط لغة المستند.

```csharp
public string Language { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLanguageDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى مجموعة خصائص المستند المدمجة
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // اضبط خاصية اللغة
            builtInProperties.Language = "en-US";

            // اضبط خصائص أساسية أخرى للتوضيح
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Language Property Demo";

            // احفظ المصنف
            workbook.Save("LanguagePropertyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


