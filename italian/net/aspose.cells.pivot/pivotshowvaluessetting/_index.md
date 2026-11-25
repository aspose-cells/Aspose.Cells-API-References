---
title: "Classe PivotShowValuesSetting"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Pivot.PivotShowValuesSetting. Rappresenta le impostazioni per la visualizzazione dei valori quando il calcolo ShowDataAs è in uso"
type: docs
url: /it/net/aspose.cells.pivot/pivotshowvaluessetting/
---
## PivotShowValuesSetting class

Rappresenta le impostazioni per la visualizzazione dei valori quando è in uso il calcolo ShowDataAs.

```csharp
public class PivotShowValuesSetting
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BaseFieldIndex](../../aspose.cells.pivot/pivotshowvaluessetting/basefieldindex/) { get; set; } | Rappresenta il campo base per un calcolo ShowDataAs quando il calcolo ShowDataAs è in uso. |
| [BaseFieldName](../../aspose.cells.pivot/pivotshowvaluessetting/basefieldname/) { get; } | Ottiene la didascalia del campo base pivot. |
| [BaseItemCaption](../../aspose.cells.pivot/pivotshowvaluessetting/baseitemcaption/) { get; } | Ottiene la didascalia dell'elemento pivot nel campo base. |
| [BaseItemIndex](../../aspose.cells.pivot/pivotshowvaluessetting/baseitemindex/) { get; set; } | Rappresenta l'indice personalizzato dell'elemento pivot nel campo base quando il calcolo ShowDataAs è in uso. |
| [BaseItemPositionType](../../aspose.cells.pivot/pivotshowvaluessetting/baseitempositiontype/) { get; set; } | (**Obsolete.**) Rappresenta il tipo dell'elemento pivot base nel campo base quando il calcolo ShowDataAs è in uso. Poiché PivotItemPosition.Custom è solo in lettura, se è necessario impostare PivotItemPosition.Custom, impostare l'attributo PivotField.BaseItemIndex. |
| [CalculationType](../../aspose.cells.pivot/pivotshowvaluessetting/calculationtype/) { get; set; } | (**Obsolete.**) Rappresenta come visualizzare i valori di un campo dati nel report pivot. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotshowvaluessetting/showvaluesas/) { get; set; } | Ottiene e imposta come visualizzare i valori di un campo dati nel report pivot. |

## Campi

| Nome | Descrizione |
| --- | --- |
| const [NextPivotItem](../../aspose.cells.pivot/pivotshowvaluessetting/nextpivotitem/) | Indice speciale dell'elemento base: utilizza l'elemento pivot successivo. Valido per i calcoli "Show Values As"; efficace in Excel 2010 e versioni successive. |
| const [PreviousPivotItem](../../aspose.cells.pivot/pivotshowvaluessetting/previouspivotitem/) | Indice speciale dell'elemento base: utilizza l'elemento pivot precedente. Valido per i calcoli "Show Values As"; efficace in Excel 2010 e versioni successive. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotShowValuesSettingDemo
    {
        public static void PivotShowValuesSettingExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells[0, 0].Value = "Product";
            worksheet.Cells[0, 1].Value = "Sales";
            worksheet.Cells[1, 0].Value = "A";
            worksheet.Cells[1, 1].Value = 100;
            worksheet.Cells[2, 0].Value = "B";
            worksheet.Cells[2, 1].Value = 150;
            worksheet.Cells[3, 0].Value = "C";
            worksheet.Cells[3, 1].Value = 200;

            // Aggiungi una tabella pivot al foglio di lavoro
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // Accedi al campo dati
            PivotField dataField = pivotTable.DataFields[0];

            // Accedi alla proprietà ShowValuesSetting
            PivotShowValuesSetting showValuesSetting = dataField.ShowValuesSetting;

            // Imposta le proprietà di PivotShowValuesSetting
            showValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
            showValuesSetting.BaseFieldIndex = 0; // Base field index
            showValuesSetting.BaseItemPositionType = PivotItemPositionType.Next;
            showValuesSetting.BaseItemIndex = 1; // Base item index

            // Aggiorna e calcola i dati della tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotShowValuesSettingExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


