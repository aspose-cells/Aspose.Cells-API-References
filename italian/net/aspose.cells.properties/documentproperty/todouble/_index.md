---
title: "DocumentProperty.ToDouble"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo DocumentProperty. Restituisce il valore della proprietà come double"
type: docs
url: /it/net/aspose.cells.properties/documentproperty/todouble/
---
## DocumentProperty.ToDouble method

Restituisce il valore della proprietà come double.

```csharp
public double ToDouble()
```

### Osservazioni

Genera un'eccezione se il tipo della proprietà non è PropertyType.Float.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToDoubleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Ottieni la collezione delle proprietà documento personalizzate
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Aggiungi una proprietà numerica
            customProperties.Add("Rating", 4.75);

            // Ottieni la proprietà e converti in double
            DocumentProperty ratingProperty = customProperties["Rating"];
            double ratingValue = ratingProperty.ToDouble();

            // Restituisci il risultato
            Console.WriteLine($"Rating: {ratingValue}");

            // Salva la cartella di lavoro
            workbook.Save("DocumentPropertyToDoubleExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


