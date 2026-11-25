---
title: "DocumentProperty.ToDateTime"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo DocumentProperty. Restituisce il valore della proprietà come DateTime nel fuso orario locale"
type: docs
url: /it/net/aspose.cells.properties/documentproperty/todatetime/
---
## DocumentProperty.ToDateTime method

Restituisce il valore della proprietà come DateTime nel fuso orario locale.

```csharp
public DateTime ToDateTime()
```

### Osservazioni

Lancia un'eccezione se il tipo della proprietà non è PropertyType.Date.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToDateTimeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Ottieni la collezione delle proprietà documento personalizzate
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Aggiungi una proprietà datetime
            DateTime currentTime = DateTime.Now;
            customProperties.Add("LastModified", currentTime);

            // Ottieni la proprietà e converti in DateTime
            DocumentProperty lastModifiedProperty = customProperties["LastModified"];
            DateTime retrievedTime = lastModifiedProperty.ToDateTime();

            // Restituisci il risultato
            Console.WriteLine($"Stored DateTime: {currentTime}");
            Console.WriteLine($"Retrieved DateTime: {retrievedTime}");

            // Salva la cartella di lavoro
            workbook.Save("DocumentPropertyDateTimeExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


