---
title: "BuiltInDocumentPropertyCollection.Characters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "BuiltInDocumentPropertyCollection property. Rappresenta una stima del numero di caratteri nel documento"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/characters/
---
## BuiltInDocumentPropertyCollection.Characters property

Rappresenta una stima del numero di caratteri nel documento.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Characters { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyCharactersDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alle proprietà del documento integrate
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Visualizza il valore corrente di Characters (proprietà obsoleta)
            Console.WriteLine("Current Characters value: " + properties.Characters);

            // Imposta un nuovo valore per Characters (proprietà obsoleta)
            properties.Characters = 1500;
            Console.WriteLine("Updated Characters value: " + properties.Characters);

            // Aggiungi del contenuto per dimostrare l'effetto della proprietà
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample text to demonstrate document properties.");
            
            // Salva la cartella di lavoro
            workbook.Save("PropertyCharactersDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


