---
title: "Workbook.ContentTypeProperties"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Workbook. Ottiene l'elenco degli oggetti ContentTypeProperty nella cartella di lavoro"
type: docs
url: /it/net/aspose.cells/workbook/contenttypeproperties/
---
## Workbook.ContentTypeProperties property

Ottiene l'elenco degli oggetti [`ContentTypeProperty`](../../../aspose.cells.properties/contenttypeproperty/) nella cartella di lavoro.

```csharp
public ContentTypePropertyCollection ContentTypeProperties { get; }
```

### Esempi

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
            
            // Aggiungi una proprietà stringa semplice
            int index1 = workbook.ContentTypeProperties.Add("Property1", "Sample Value");
            workbook.ContentTypeProperties[index1].IsNillable = true;
            
            // Aggiungi una proprietà datetime con specifica del tipo
            int index2 = workbook.ContentTypeProperties.Add("Property2", 
                DateTime.Now.ToString("yyyy-MM-ddTHH:mm:ss"), "DateTime");
            workbook.ContentTypeProperties[index2].IsNillable = false;
            
            // Salva la cartella di lavoro
            workbook.Save("ContentTypePropertiesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ContentTypePropertyCollection](../../../aspose.cells.properties/contenttypepropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


