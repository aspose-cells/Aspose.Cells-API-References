---
title: "BuiltInDocumentPropertyCollection.Keywords"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية BuiltInDocumentPropertyCollection. تحصل أو تضبط الكلمات المفتاحية للمستند"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/keywords/
---
## BuiltInDocumentPropertyCollection.Keywords property

يحصل أو يعيّن كلمات مفتاحية للمستند.

```csharp
public string Keywords { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyKeywordsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // اضبط خاصية Keywords
            workbook.BuiltInDocumentProperties.Keywords = "Sample Keywords, Aspose.Cells, Demo";
            
            // احفظ المصنف
            workbook.Save("output_keywords.xlsx");
            
            // حمّل دفتر العمل المحفوظ للتحقق من خاصية Keywords
            Workbook loadedWorkbook = new Workbook("output_keywords.xlsx");
            
            // اعرض خاصية Keywords
            Console.WriteLine("Document Keywords: " + loadedWorkbook.BuiltInDocumentProperties.Keywords);
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


