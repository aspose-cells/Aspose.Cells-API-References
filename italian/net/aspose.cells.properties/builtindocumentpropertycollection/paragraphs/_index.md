---
title: "BuiltInDocumentPropertyCollection.Paragraphs"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "BuiltInDocumentPropertyCollection property. Rappresenta una stima del numero di paragrafi nel documento"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/paragraphs/
---
## BuiltInDocumentPropertyCollection.Paragraphs property

Rappresenta una stima del numero di paragrafi nel documento.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Paragraphs { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyParagraphsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alle proprietà del documento integrate
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Visualizza il valore corrente di Paragraphs (proprietà obsoleta)
            Console.WriteLine("Current Paragraphs value: " + properties.Paragraphs);

            // Imposta un nuovo valore per Paragraphs (proprietà obsoleta)
            properties.Paragraphs = 15;
            Console.WriteLine("Updated Paragraphs value: " + properties.Paragraphs);

            // Aggiungi del contenuto per dimostrare l'effetto della proprietà
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is paragraph 1");
            worksheet.Cells["A2"].PutValue("This is paragraph 2");
            worksheet.Cells["A3"].PutValue("This is paragraph 3");

            // Salva la cartella di lavoro
            workbook.Save("PropertyParagraphsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


