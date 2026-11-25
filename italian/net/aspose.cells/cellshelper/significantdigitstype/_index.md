---
title: "CellsHelper.SignificantDigitsType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellsHelper. Ottiene e imposta il tipo predefinito di cifre significative per la visualizzazione dei valori numerici. Il valore predefinito è G17"
type: docs
url: /it/net/aspose.cells/cellshelper/significantdigitstype/
---
## CellsHelper.SignificantDigitsType property

Ottiene e imposta il tipo predefinito di cifre significative per l'emissione di valori numerici. Il valore predefinito è G17.

```csharp
public static SignificantDigitsType SignificantDigitsType { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperPropertySignificantDigitsTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Visualizza il valore corrente di SignificantDigitsType
                Console.WriteLine("Current SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Imposta un nuovo valore di SignificantDigitsType
                CellsHelper.SignificantDigitsType = SignificantDigitsType.G17;
                Console.WriteLine("Updated SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Crea una cartella di lavoro per dimostrare l'effetto
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Aggiungi un valore numerico che sarà influenzato dalle cifre significative
                worksheet.Cells["A1"].PutValue(1.2345678912345678);
                worksheet.Cells["A2"].PutValue(1.2345678912345678);
                worksheet.Cells["A3"].Formula = "=A1+A2";

                // Calcola le formule con il tipo corrente di cifre significative
                workbook.CalculateFormula();

                // Visualizza il risultato
                Console.WriteLine("Calculation result: " + worksheet.Cells["A3"].Value);

                // Passa a un altro tipo di cifre significative
                CellsHelper.SignificantDigitsType = SignificantDigitsType.Rounding17;
                Console.WriteLine("Changed SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Ricalcola con il nuovo tipo di cifre significative
                workbook.CalculateFormula();
                Console.WriteLine("Recalculated result: " + worksheet.Cells["A3"].Value);

                // Salva la cartella di lavoro
                workbook.Save("SignificantDigitsTypeDemo.xlsx");
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

* enum [SignificantDigitsType](../../significantdigitstype/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


