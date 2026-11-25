---
title: "Enumerazione PivotTableAutoFormatType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enumerazione Aspose.Cells.Pivot.PivotTableAutoFormatType. Rappresenta il tipo di formattazione automatica della PivotTable"
type: docs
url: /it/net/aspose.cells.pivot/pivottableautoformattype/
---
## PivotTableAutoFormatType enumeration

Rappresenta il tipo di formato automatico della PivotTable.

```csharp
public enum PivotTableAutoFormatType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Rappresenta il tipo di formato Nessuno. |
| Classic | `1` | Rappresenta il tipo di formato automatico Classico. |
| Report1 | `2` | Rappresenta il tipo di formato Report1. |
| Report2 | `3` | Rappresenta il tipo di formato Report2. |
| Report3 | `4` | Rappresenta il tipo di formato Report3. |
| Report4 | `5` | Rappresenta il tipo di formato Report4. |
| Report5 | `6` | Rappresenta il tipo di formato Report5. |
| Report6 | `7` | Rappresenta il tipo di formato Report6. |
| Report7 | `8` | Rappresenta il tipo di formato Report7. |
| Report8 | `9` | Rappresenta il tipo di formato Report8. |
| Report9 | `10` | Rappresenta il tipo di formato Report9. |
| Report10 | `11` | Rappresenta il tipo di formato Report10. |
| Table1 | `12` | Rappresenta il tipo di formato Table1. |
| Table2 | `13` | Rappresenta il tipo di formato Table2. |
| Table3 | `14` | Rappresenta il tipo di formato Table3. |
| Table4 | `15` | Rappresenta il tipo di formato Table4. |
| Table5 | `16` | Rappresenta il tipo di formato Table5. |
| Table6 | `17` | Rappresenta il tipo di formato Table6. |
| Table7 | `18` | Rappresenta il tipo di formato Table7. |
| Table8 | `19` | Rappresenta il tipo di formato Table8. |
| Table9 | `20` | Rappresenta il tipo di formato Table9. |
| Table10 | `21` | Rappresenta il tipo di formato Table10. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableAutoFormatTypeDemo
    {
        public static void PivotTableAutoFormatTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio per la PivotTable
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 0].Value = "Apple";
            worksheet.Cells[3, 1].Value = 2021;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 0].Value = "Banana";
            worksheet.Cells[4, 1].Value = 2021;
            worksheet.Cells[4, 2].Value = 80;

            // Aggiungi una PivotTable al foglio di lavoro
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi alla PivotTable
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Imposta il tipo di formato automatico per la PivotTable
            pivotTable.AutoFormatType = PivotTableAutoFormatType.Report1;

            // Salva la cartella di lavoro
            workbook.Save("PivotTableAutoFormatTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


