---
title: "BuiltInDocumentPropertyCollection.CharactersWithSpaces"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Rappresenta una stima del numero di caratteri, spazi inclusi, nel documento"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/characterswithspaces/
---
## BuiltInDocumentPropertyCollection.CharactersWithSpaces property

Rappresenta una stima del numero di caratteri (spazi inclusi) nel documento.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CharactersWithSpaces { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyCharactersWithSpacesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alle proprietà del documento integrate
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Visualizza il valore corrente di CharactersWithSpaces
            Console.WriteLine("Current CharactersWithSpaces value: " + properties.CharactersWithSpaces);
            
            // Imposta un nuovo valore per CharactersWithSpaces
            properties.CharactersWithSpaces = 1500;
            Console.WriteLine("Updated CharactersWithSpaces value: " + properties.CharactersWithSpaces);
            
            // Aggiungi del contenuto per dimostrare l'effetto della proprietà
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample text to demonstrate document properties.");
            worksheet.Cells["A2"].PutValue("The CharactersWithSpaces property represents estimated character count including spaces.");
            
            // Salva la cartella di lavoro
            workbook.Save("PropertyCharactersWithSpacesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


