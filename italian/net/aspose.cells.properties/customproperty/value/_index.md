---
title: "CustomProperty.Value"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "CustomProperty proprietà. Restituisce o imposta il valore della proprietà personalizzata"
type: docs
url: /it/net/aspose.cells.properties/customproperty/value/
---
## CustomProperty.Value property

Restituisce o imposta il valore della proprietà personalizzata.

```csharp
public string Value { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomPropertyPropertyValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una proprietà personalizzata con un valore stringa lungo
            worksheet.CustomProperties.Add("VeryLongString", "This is a very long string value for testing custom properties");
            
            // Ottieni e visualizza il valore della proprietà personalizzata
            string propertyValue = worksheet.CustomProperties["VeryLongString"].Value;
            Console.WriteLine("Custom Property Value: " + propertyValue);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Ricarica la cartella di lavoro per verificare che la proprietà persista
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Verifica che il valore sia lo stesso dopo il caricamento
            string loadedValue = loadedWorksheet.CustomProperties["VeryLongString"].Value;
            Console.WriteLine("Reloaded Custom Property Value: " + loadedValue);
        }
    }
}
```

### Vedi anche

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


