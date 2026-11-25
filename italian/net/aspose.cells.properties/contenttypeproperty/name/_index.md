---
title: "ContentTypeProperty.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ContentTypeProperty. Restituisce o imposta il nome dell'oggetto"
type: docs
url: /it/net/aspose.cells.properties/contenttypeproperty/name/
---
## ContentTypeProperty.Name property

Restituisce o imposta il nome dell'oggetto.

```csharp
public string Name { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi una proprietà di tipo contenuto con nome "ss"
            workbook.ContentTypeProperties.Add("ss", "bb", "text");
            
            // Salva in formato XLS
            workbook.Save("example.xls");
            
            // Ricarica la cartella di lavoro e verifica la proprietà Name
            workbook = new Workbook("example.xls");
            Console.WriteLine("Name property in XLS: " + workbook.ContentTypeProperties[0].Name);
            
            // Salva in formato XLSX
            workbook.Save("example.xlsx");
            
            // Ricarica e verifica di nuovo
            workbook = new Workbook("example.xlsx");
            Console.WriteLine("Name property in XLSX: " + workbook.ContentTypeProperties[0].Name);
        }
    }
}
```

### Vedi anche

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


