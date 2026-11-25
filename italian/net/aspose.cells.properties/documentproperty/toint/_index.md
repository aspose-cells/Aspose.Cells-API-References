---
title: "DocumentProperty.ToInt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo DocumentProperty. Restituisce il valore della proprietà come intero"
type: docs
url: /it/net/aspose.cells.properties/documentproperty/toint/
---
## DocumentProperty.ToInt method

Restituisce il valore della proprietà come integer.

```csharp
public int ToInt()
```

### Osservazioni

Genera un'eccezione se il tipo della proprietà non è PropertyType.Number.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToIntDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Ottieni la collezione delle proprietà del documento personalizzate
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Aggiungi una proprietà personalizzata numerica
            customProperties.Add("Revision", 5);

            // Ottieni la proprietà e converti in int usando ToInt()
            DocumentProperty revisionProperty = customProperties["Revision"];
            int revisionValue = revisionProperty.ToInt();
            
            // Restituisci il risultato
            Console.WriteLine($"Revision (as int): {revisionValue}");

            // Salva la cartella di lavoro
            workbook.Save("DocumentPropertyToIntExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


