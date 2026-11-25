---
title: "Class PivotArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Pivot.PivotArea. Presenta l'area selezionata della tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotarea/
---
## PivotArea class

Presenta l'area selezionata della tabella pivot.

```csharp
public class PivotArea
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PivotArea](pivotarea/)(PivotTable) | Presenta l'area selezionata della PivotTable. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AxisType](../../aspose.cells.pivot/pivotarea/axistype/) { get; set; } | Ottiene e imposta la regione della PivotTable a cui si applica questa regola. |
| [Filters](../../aspose.cells.pivot/pivotarea/filters/) { get; } | Ottiene tutti i filtri per questa PivotArea. |
| [IsColumnGrandIncluded](../../aspose.cells.pivot/pivotarea/iscolumngrandincluded/) { get; set; } | Indica se il totale generale della colonna è incluso. |
| [IsOutline](../../aspose.cells.pivot/pivotarea/isoutline/) { get; set; } | Indica se la regola si riferisce a un'area in modalità struttura. |
| [IsRowGrandIncluded](../../aspose.cells.pivot/pivotarea/isrowgrandincluded/) { get; set; } | Indica se il totale generale della riga è incluso. |
| [OnlyData](../../aspose.cells.pivot/pivotarea/onlydata/) { get; set; } | Indica se sono selezionati solo i valori dei dati (nell'area dati della visualizzazione) per una selezione di elementi e non includono le etichette degli elementi. |
| [OnlyLabel](../../aspose.cells.pivot/pivotarea/onlylabel/) { get; set; } | Indica se sono selezionate solo le etichette dei dati per una selezione di elementi. |
| [RuleType](../../aspose.cells.pivot/pivotarea/ruletype/) { get; set; } | Ottiene e imposta il tipo di regola di selezione. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetCellAreas](../../aspose.cells.pivot/pivotarea/getcellareas/)() | Ottiene le aree di celle di questa area pivot. |
| [Select](../../aspose.cells.pivot/pivotarea/select/)(PivotFieldType, int, PivotTableSelectionType) | Seleziona l'area con i filtri. |
| [SelectField](../../aspose.cells.pivot/pivotarea/selectfield/#selectfield)(PivotFieldType, PivotField) | Seleziona un campo nella regione come area. |
| [SelectField](../../aspose.cells.pivot/pivotarea/selectfield/#selectfield_1)(PivotFieldType, string) | Seleziona un campo nella regione come area. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaDemo
    {
        public static void PivotAreaExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2021;
            worksheet.Cells[3, 1].Value = 2022;
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;

            // Aggiungi una tabella pivot al foglio di lavoro
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Crea un'istanza di PivotArea
            PivotArea pivotArea = new PivotArea(pivotTable);

            // Imposta le proprietà di PivotArea
            pivotArea.OnlyData = true;
            pivotArea.OnlyLabel = false;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.IsOutline = false;

            // Usa il metodo Select per selezionare un'area specifica
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.DataAndLabel);

            // Salva la cartella di lavoro
            workbook.Save("PivotAreaExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


