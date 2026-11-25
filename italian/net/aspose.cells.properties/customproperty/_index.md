---
title: "Classe CustomProperty"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Properties.CustomProperty class. Rappresenta una proprietà personalizzata che memorizza coppie nome‑valore di dati arbitrari definiti dall'utente per il foglio di lavoro"
type: docs
url: /it/net/aspose.cells.properties/customproperty/
---
## CustomProperty class

Rappresenta una proprietà personalizzata che memorizza coppie nome‑valore di dati arbitrari definiti dall'utente per il foglio di lavoro.

```csharp
public class CustomProperty
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BinaryValue](../../aspose.cells.properties/customproperty/binaryvalue/) { get; set; } | Ottiene e imposta il valore binario della proprietà personalizzata. |
| [Name](../../aspose.cells.properties/customproperty/name/) { get; set; } | Restituisce o imposta il nome dell'oggetto. |
| [StringValue](../../aspose.cells.properties/customproperty/stringvalue/) { get; set; } | (**Obsolete.**) Restituisce o imposta il valore della proprietà personalizzata. |
| [Value](../../aspose.cells.properties/customproperty/value/) { get; set; } | Restituisce o imposta il valore della proprietà personalizzata. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyDemo
    {
        public static void CustomPropertyExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Accedi alla raccolta CustomProperties
            CustomPropertyCollection customProperties = sheet.CustomProperties;

            // Aggiungi proprietà personalizzate
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Version", "1.0");
            customProperties.Add("LastModified", DateTime.Now.ToString());

            // Accedi e visualizza le proprietà personalizzate
            for (int i = 0; i < customProperties.Count; i++)
            {
                CustomProperty property = customProperties[i];
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}");
            }

            // Salva la cartella di lavoro
            workbook.Save("CustomPropertyExample.xlsx");
            workbook.Save("CustomPropertyExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


