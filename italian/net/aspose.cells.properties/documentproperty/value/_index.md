---
title: "DocumentProperty.Value"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DocumentProperty. Ottiene o imposta il valore della proprietà"
type: docs
url: /it/net/aspose.cells.properties/documentproperty/value/
---
## DocumentProperty.Value property

Ottiene o imposta il valore della proprietà.

```csharp
public object Value { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle proprietà del documento integrate
            var hyperlinkBase = workbook.Worksheets.BuiltInDocumentProperties["HyperlinkBase"];
            hyperlinkBase.Value = "http://www.example.com";

            var title = workbook.Worksheets.BuiltInDocumentProperties["Title"];
            title.Value = "Sample Document Title";

            // Salva la cartella di lavoro
            workbook.Save("DocumentPropertiesDemo.xlsx");

            // Visualizza i valori impostati
            Console.WriteLine("HyperlinkBase: " + hyperlinkBase.Value);
            Console.WriteLine("Title: " + title.Value);
        }
    }
}
```

### Vedi anche

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


