---
title: "Enum PivotFieldDataDisplayFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Pivot.PivotFieldDataDisplayFormat enum. Rappresenta il formato di visualizzazione dei dati nel campo dati della tabella pivot."
type: docs
url: /it/net/aspose.cells.pivot/pivotfielddatadisplayformat/
---
## PivotFieldDataDisplayFormat enumeration

Rappresenta il formato di visualizzazione dei dati nel campo dati della PivotTable.

```csharp
public enum PivotFieldDataDisplayFormat
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Normal | `0` | Rappresenta il formato di visualizzazione normale. |
| DifferenceFrom | `1` | Rappresenta la differenza dal formato di visualizzazione. |
| PercentageOf | `2` | Rappresenta la percentuale del formato di visualizzazione. |
| PercentageDifferenceFrom | `3` | Rappresenta la differenza percentuale dal formato di visualizzazione. |
| RunningTotalIn | `4` | Rappresenta il totale cumulativo nel formato di visualizzazione. |
| PercentageOfRow | `5` | Rappresenta la percentuale del formato di visualizzazione della riga. |
| PercentageOfColumn | `6` | Rappresenta la percentuale del formato di visualizzazione della colonna. |
| PercentageOfTotal | `7` | Rappresenta la percentuale del formato di visualizzazione totale. |
| Index | `8` | Rappresenta il formato di visualizzazione dell'indice. |
| PercentageOfParentRowTotal | `9` | Rappresenta la percentuale del formato di visualizzazione del totale della riga padre. |
| PercentageOfParentColumnTotal | `10` | Rappresenta la percentuale del formato di visualizzazione del totale della colonna padre. |
| PercentageOfParentTotal | `11` | Rappresenta la percentuale del formato di visualizzazione del totale padre. |
| PercentageOfRunningTotalIn | `12` | Rappresenta la percentuale del totale cumulativo nel formato di visualizzazione. |
| RankSmallestToLargest | `13` | Rappresenta il formato di visualizzazione dal più piccolo al più grande. |
| RankLargestToSmallest | `14` | Rappresenta il formato di visualizzazione dal più grande al più piccolo. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldDataDisplayFormatDemo
    {
        public static void PivotFieldDataDisplayFormatExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Aggiungi alcuni dati di esempio
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Aggiungi una tabella pivot
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Imposta lo stile della tabella pivot
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Modifica gli attributi del PivotField
            PivotField dataField = pivot.DataFields[0];
            dataField.DisplayName = "custom display name";

            // Imposta DataDisplayFormat
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;

            // Aggiorna e calcola i dati
            pivot.RefreshData();
            pivot.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotFieldDataDisplayFormatExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


