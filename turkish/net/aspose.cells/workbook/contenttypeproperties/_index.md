---
title: "Workbook.ContentTypeProperties"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Çalışma kitabındaki ContentTypeProperty nesnelerinin listesini alır"
type: docs
url: /tr/net/aspose.cells/workbook/contenttypeproperties/
---
## Workbook.ContentTypeProperties property

Çalışma kitabındaki [`ContentTypeProperty`](../../../aspose.cells.properties/contenttypeproperty/) nesnelerinin listesini alır.

```csharp
public ContentTypePropertyCollection ContentTypeProperties { get; }
```

### Örnekler

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
            
            // Basit bir dize özelliği ekle
            int index1 = workbook.ContentTypeProperties.Add("Property1", "Sample Value");
            workbook.ContentTypeProperties[index1].IsNillable = true;
            
            // Tür belirtimiyle datetime özelliği ekle
            int index2 = workbook.ContentTypeProperties.Add("Property2", 
                DateTime.Now.ToString("yyyy-MM-ddTHH:mm:ss"), "DateTime");
            workbook.ContentTypeProperties[index2].IsNillable = false;
            
            // Çalışma kitabını kaydedin
            workbook.Save("ContentTypePropertiesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ContentTypePropertyCollection](../../../aspose.cells.properties/contenttypepropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


