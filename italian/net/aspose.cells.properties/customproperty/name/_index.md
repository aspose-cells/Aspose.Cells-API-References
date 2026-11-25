---
title: "CustomProperty.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "CustomProperty proprietà. Restituisce o imposta il nome dell'oggetto"
type: docs
url: /it/net/aspose.cells.properties/customproperty/name/
---
## CustomProperty.Name property

Restituisce o imposta il nome dell'oggetto.

```csharp
public string Name { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi una proprietà personalizzata con un nome e un valore
                worksheet.CustomProperties.Add("SampleName", "SampleValue");

                // Recupera la proprietà personalizzata
                CustomProperty customProperty = worksheet.CustomProperties["SampleName"];

                // Visualizza il valore corrente della proprietà Name (operazione di lettura)
                Console.WriteLine("Custom Property Name: " + customProperty.Name);

                // Imposta un nuovo valore per la proprietà Name
                customProperty.Name = "UpdatedName";
                Console.WriteLine("Updated Custom Property Name: " + customProperty.Name);

                // Salva la cartella di lavoro
                workbook.Save("NameDemo.xlsx");
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


