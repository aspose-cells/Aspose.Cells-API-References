---
title: "CustomProperty.StringValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "CustomProperty proprietà. Restituisce o imposta il valore della proprietà personalizzata"
type: docs
url: /it/net/aspose.cells.properties/customproperty/stringvalue/
---
## CustomProperty.StringValue property

Restituisce o imposta il valore della proprietà personalizzata.

```csharp
[Obsolete("Use CustomProperty.Value property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StringValue { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà CustomProperty.Value. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2010. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyStringValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi una proprietà personalizzata con un valore stringa
                worksheet.CustomProperties.Add("SampleProperty", "Test Value");

                // Recupera la proprietà personalizzata
                CustomProperty customProperty = worksheet.CustomProperties["SampleProperty"];

                // Visualizza la proprietà StringValue (operazione di lettura)
                Console.WriteLine("StringValue: " + customProperty.StringValue);

                // Imposta un nuovo valore per la proprietà StringValue
                customProperty.StringValue = "Updated Value";
                Console.WriteLine("Updated StringValue: " + customProperty.StringValue);

                // Salva la cartella di lavoro
                workbook.Save("StringValueDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


