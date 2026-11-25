---
title: "Classe CellValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.CellValue. Rappresenta il valore della cella e il tipo corrispondente"
type: docs
url: /it/net/aspose.cells/cellvalue/
---
## CellValue class

Rappresenta il valore della cella e il tipo corrispondente.

```csharp
public class CellValue
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [CellValue](cellvalue/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Type](../../aspose.cells/cellvalue/type/) { get; set; } | Ottiene o imposta il tipo di valore della cella. |
| [Value](../../aspose.cells/cellvalue/value/) { get; set; } | Ottiene o imposta il valore della cella. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueDemo
    {
        public static void CellValueExample()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di CellValue
            CellValue cellValue = new CellValue();

            // Imposta il tipo e il valore della cella
            cellValue.Type = CellValueType.IsNumeric;
            cellValue.Value = 123.45;

            // Assegna il CellValue a una cella nel foglio di lavoro
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(cellValue.Value);

            // Salva la cartella di lavoro
            workbook.Save("CellValueExample.xlsx");
            workbook.Save("CellValueExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


