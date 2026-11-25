---
title: "FontConfigs.IsFontAvailable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FontConfigs. Indica se il carattere è disponibile"
type: docs
url: /it/net/aspose.cells/fontconfigs/isfontavailable/
---
## FontConfigs.IsFontAvailable method

Indica se il carattere è disponibile.

```csharp
public static bool IsFontAvailable(string fontName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontName | String | nome del font |

### Valore di ritorno

true se il carattere è disponibile, altrimenti false.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodIsFontAvailableWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Testa i nomi dei caratteri per verificarne la disponibilità
            string[] testFonts = { "Arial", "Times New Roman", "NonExistentFont" };

            try
            {
                foreach (string fontName in testFonts)
                {
                    // Chiama il metodo IsFontAvailable con il nome del carattere
                    bool isAvailable = FontConfigs.IsFontAvailable(fontName);

                    // Visualizza il risultato
                    Console.WriteLine($"Font '{fontName}' is available: {isAvailable}");

                    // Scrivi il risultato nel foglio di lavoro
                    int row = worksheet.Cells.MaxDataRow + 1;
                    worksheet.Cells[row, 0].PutValue($"Font '{fontName}' available:");
                    worksheet.Cells[row, 1].PutValue(isAvailable);
                }

                Console.WriteLine("Method executed successfully with parameters (String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsFontAvailable method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("FontConfigsMethodIsFontAvailableWithStringDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


