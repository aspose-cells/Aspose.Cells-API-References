---
title: "Workbook.ContentTypeProperties"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تحصل على قائمة كائنات ContentTypeProperty في دفتر العمل"
type: docs
url: /ar/net/aspose.cells/workbook/contenttypeproperties/
---
## Workbook.ContentTypeProperties property

يحصل على قائمة كائنات [`ContentTypeProperty`](../../../aspose.cells.properties/contenttypeproperty/) في دفتر العمل.

```csharp
public ContentTypePropertyCollection ContentTypeProperties { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyContentTypePropertiesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // إضافة خاصية سلسلة بسيطة
            int index1 = workbook.ContentTypeProperties.Add("Property1", "Sample Value");
            workbook.ContentTypeProperties[index1].IsNillable = true;
            
            // إضافة خاصية datetime مع تحديد النوع
            int index2 = workbook.ContentTypeProperties.Add("Property2", 
                DateTime.Now.ToString("yyyy-MM-ddTHH:mm:ss"), "DateTime");
            workbook.ContentTypeProperties[index2].IsNillable = false;
            
            // احفظ المصنف
            workbook.Save("ContentTypePropertiesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ContentTypePropertyCollection](../../../aspose.cells.properties/contenttypepropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


