---
title: "Workbook.ContentTypeProperties"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Workbook. Obtiene la lista de objetos ContentTypeProperty en el libro de trabajo"
type: docs
url: /es/net/aspose.cells/workbook/contenttypeproperties/
---
## Workbook.ContentTypeProperties property

Obtiene la lista de objetos [`ContentTypeProperty`](../../../aspose.cells.properties/contenttypeproperty/) en el libro de trabajo.

```csharp
public ContentTypePropertyCollection ContentTypeProperties { get; }
```

### Ejemplos

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
            
            // Agregar una propiedad de cadena simple
            int index1 = workbook.ContentTypeProperties.Add("Property1", "Sample Value");
            workbook.ContentTypeProperties[index1].IsNillable = true;
            
            // Agregar una propiedad datetime con especificación de tipo
            int index2 = workbook.ContentTypeProperties.Add("Property2", 
                DateTime.Now.ToString("yyyy-MM-ddTHH:mm:ss"), "DateTime");
            workbook.ContentTypeProperties[index2].IsNillable = false;
            
            // Guarda el libro de trabajo
            workbook.Save("ContentTypePropertiesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ContentTypePropertyCollection](../../../aspose.cells.properties/contenttypepropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


