---
title: "CustomProperty.BinaryValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CustomProperty. Ottiene e imposta il valore binario della proprietà personalizzata"
type: docs
url: /it/net/aspose.cells.properties/customproperty/binaryvalue/
---
## CustomProperty.BinaryValue property

Ottiene e imposta il valore binario della proprietà personalizzata.

```csharp
public byte[] BinaryValue { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyBinaryValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una proprietà personalizzata con un valore di esempio
            worksheet.CustomProperties.Add("SampleBinary", "01010101");

            try
            {
                // Recupera la proprietà personalizzata
                CustomProperty prop = worksheet.CustomProperties["SampleBinary"];

                // Visualizza il Nome e il Valore della proprietà personalizzata
                Console.WriteLine($"Custom Property Name : {prop.Name}");
                Console.WriteLine($"Custom Property Value: {prop.Value}");

                // NOTA: Il riflesso per CustomProperty non include una proprietà BinaryValue.
                // Il valore disponibile basato su stringa è accessibile tramite la proprietà 'Value'.

                // Salva la cartella di lavoro (opzionale)
                workbook.Save("BinaryValueDemo.xlsx");
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


