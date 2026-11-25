---
title: "BuiltInDocumentPropertyCollection.Lines"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Rappresenta una stima del numero di righe nel documento"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/lines/
---
## BuiltInDocumentPropertyCollection.Lines property

Rappresenta una stima del numero di righe nel documento.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Lines { get; set; }
```

### Osservazioni

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyLinesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alle proprietà del documento integrate
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Visualizza il valore corrente di Lines (stima del numero di righe nel documento)
            Console.WriteLine("Current Lines value: " + properties.Lines);
            
            // Imposta un nuovo valore per la proprietà Lines
            properties.Lines = 150;
            
            // Aggiungi del contenuto per dimostrare lo scopo della proprietà
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Line " + (i + 1);
            }
            
            // Salva la cartella di lavoro
            workbook.Save("PropertyLinesDemo.xlsx");
            
            // Nota: la proprietà Lines è una stima e non si aggiornerà automaticamente con il contenuto reale
            // È principalmente usata per scopi di metadati del documento
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


