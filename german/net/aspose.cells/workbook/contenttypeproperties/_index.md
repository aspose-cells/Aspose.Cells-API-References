---
title: "Workbook.ContentTypeProperties"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Eigenschaft. Gibt die Liste der ContentTypeProperty-Objekte im Arbeitsbuch zurück"
type: docs
url: /de/net/aspose.cells/workbook/contenttypeproperties/
---
## Workbook.ContentTypeProperties property

Gibt die Liste der [`ContentTypeProperty`](../../../aspose.cells.properties/contenttypeproperty/) Objekte im Arbeitsbuch zurück.

```csharp
public ContentTypePropertyCollection ContentTypeProperties { get; }
```

### Beispiele

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
            
            // Einfaches Zeichenketten-Property hinzufügen
            int index1 = workbook.ContentTypeProperties.Add("Property1", "Sample Value");
            workbook.ContentTypeProperties[index1].IsNillable = true;
            
            // Datetime-Property mit Typangabe hinzufügen
            int index2 = workbook.ContentTypeProperties.Add("Property2", 
                DateTime.Now.ToString("yyyy-MM-ddTHH:mm:ss"), "DateTime");
            workbook.ContentTypeProperties[index2].IsNillable = false;
            
            // Speichere die Arbeitsmappe
            workbook.Save("ContentTypePropertiesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ContentTypePropertyCollection](../../../aspose.cells.properties/contenttypepropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


