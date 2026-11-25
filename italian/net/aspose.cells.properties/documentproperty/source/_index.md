---
title: "DocumentProperty.Source"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DocumentProperty. La fonte del contenuto collegato"
type: docs
url: /it/net/aspose.cells.properties/documentproperty/source/
---
## DocumentProperty.Source property

L'origine del contenuto collegato.

```csharp
public string Source { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertySourceDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alle proprietà personalizzate del documento
            var properties = workbook.Worksheets.CustomDocumentProperties;

            // Aggiungi proprietà
            properties.Add("Author", "John Doe");
            properties.Add("CreatedDate", DateTime.Now);
            properties.Add("Revision", 1);
            
            // Ottieni le proprietà e visualizza le loro fonti
            Console.WriteLine("Property Sources:");
            Console.WriteLine($"Author: {properties["Author"].Source}");
            Console.WriteLine($"CreatedDate: {properties["CreatedDate"].Source}");
            Console.WriteLine($"Revision: {properties["Revision"].Source}");

            // Salva la cartella di lavoro
            workbook.Save("DocumentPropertiesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


