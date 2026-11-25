---
title: "Enum CellValueFormatStrategy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.CellValueFormatStrategy. Specifica come applicare lo stile al valore della cella"
type: docs
url: /it/net/aspose.cells/cellvalueformatstrategy/
---
## CellValueFormatStrategy enumeration

Specifica come applicare lo stile al valore della cella.

```csharp
public enum CellValueFormatStrategy
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Non formattato. |
| CellStyle | `1` | Solo formattato con lo stile originale della cella. |
| DisplayStyle | `2` | Formattato con lo stile visualizzato della cella. |
| DisplayString | `3` | Ottiene la stringa visualizzata mostrata in MS Excel. La principale differenza rispetto a DisplayStyle è che questa opzione considera anche l'effetto della larghezza della colonna. Se la larghezza della colonna è troppo piccola per mostrare completamente la stringa formattata, può essere mostrato "#", proprio come fa MS Excel. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueFormatStrategyDemo
    {
        public static void CellValueFormatStrategyExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B1"].PutValue("Number");
            worksheet.Cells["B2"].PutValue(12345.6789);
            worksheet.Cells["C1"].PutValue("Text");
            worksheet.Cells["C2"].PutValue("Hello World");

            // Applica diverse CellValueFormatStrategy per dimostrare i loro effetti
            // Nessuno: Non formattato
            string valueNone = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.None);
            Console.WriteLine($"None: {valueNone}");

            // CellStyle: Solo formattato con lo stile originale della cella
            string valueCellStyle = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.CellStyle);
            Console.WriteLine($"CellStyle: {valueCellStyle}");

            // DisplayStyle: Formattato con lo stile visualizzato della cella
            string valueDisplayStyle = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.DisplayStyle);
            Console.WriteLine($"DisplayStyle: {valueDisplayStyle}");

            // DisplayString: Ottiene la stringa visualizzata mostrata in MS Excel
            string valueDisplayString = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.DisplayString);
            Console.WriteLine($"DisplayString: {valueDisplayString}");

            // Salva la cartella di lavoro in un file
            workbook.Save("CellValueFormatStrategyExample.xlsx");
            workbook.Save("CellValueFormatStrategyExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


