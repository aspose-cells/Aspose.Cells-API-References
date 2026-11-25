---
title: "Enum SignificantDigitsType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.SignificantDigitsType enum. Rappresenta il tipo di cifre significative per la visualizzazione dei valori numerici"
type: docs
url: /it/net/aspose.cells/significantdigitstype/
---
## SignificantDigitsType enumeration

Rappresenta il tipo di cifre significative per l'emissione di valori numerici.

```csharp
public enum SignificantDigitsType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Digits15 | `0` | 15 cifre |
| G17 | `1` | 17 cifre formattando il valore con "G17". |
| Rounding17 | `2` | 17 cifre arrotondando il valore. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassSignificantDigitsTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un nuovo workbook per la dimostrazione
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Dimostra l'uso di ciascun valore dell'enum SignificantDigitsType
                SignificantDigitsType[] types = {
                    SignificantDigitsType.Digits15,
                    SignificantDigitsType.G17,
                    SignificantDigitsType.Rounding17
                };

                foreach (SignificantDigitsType type in types)
                {
                    // Imposta il tipo di cifre significative per la cartella di lavoro
                    workbook.Settings.SignificantDigitsType = type;

                    // Visualizza l'impostazione corrente
                    Console.WriteLine($"Current SignificantDigitsType: {type} (Value: {(int)type})");

                    // Aggiungi un valore di esempio per dimostrare l'impostazione
                    worksheet.Cells["A1"].PutValue(123.4567890123456789);

                    // Salva la cartella di lavoro con l'impostazione corrente
                    string fileName = $"SignificantDigitsType_{type}.xlsx";
                    workbook.Save(fileName);
                    Console.WriteLine($"Workbook saved with {type} setting as {fileName}");
                }

                Console.WriteLine("All SignificantDigitsType demonstrations completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating SignificantDigitsType: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


