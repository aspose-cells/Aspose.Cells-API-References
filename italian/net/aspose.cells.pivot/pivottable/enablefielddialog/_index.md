---
title: "PivotTable.EnableFieldDialog"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se la finestra di dialogo Campo PivotTable è disponibile quando l'utente fa doppio clic sul campo della PivotTable"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/enablefielddialog/
---
## PivotTable.EnableFieldDialog property

Indica se la finestra di dialogo Campo PivotTable è disponibile quando l'utente fa doppio clic sul campo PivotTable.

```csharp
public bool EnableFieldDialog { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyEnableFieldDialogDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            var cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Dimostra la proprietà EnableFieldDialog
            pivotTable.EnableFieldDialog = true;
            Console.WriteLine("EnableFieldDialog set to: " + pivotTable.EnableFieldDialog);

            // Modifica la proprietà e verifica
            pivotTable.EnableFieldDialog = false;
            Console.WriteLine("EnableFieldDialog changed to: " + pivotTable.EnableFieldDialog);

            // Salva la cartella di lavoro
            workbook.Save("PivotTable_EnableFieldDialog_Example.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


