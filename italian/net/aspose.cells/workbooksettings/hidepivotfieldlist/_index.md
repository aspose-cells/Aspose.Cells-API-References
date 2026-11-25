---
title: "WorkbookSettings.HidePivotFieldList"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene e imposta se nascondere l'elenco dei campi per la PivotTable"
type: docs
url: /it/net/aspose.cells/workbooksettings/hidepivotfieldlist/
---
## WorkbookSettings.HidePivotFieldList property

Ottiene e imposta se nascondere l'elenco dei campi per la PivotTable.

```csharp
public bool HidePivotFieldList { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyHidePivotFieldListDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["A4"].PutValue("A");
            sheet.Cells["B4"].PutValue(150);

            // Crea tabella pivot
            int index = workbook.Worksheets.Add(SheetType.Worksheet);
            Worksheet pivotSheet = workbook.Worksheets[index];
            pivotSheet.Name = "PivotTable";
            
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable", "A1:B4", "C3");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Accedi alle impostazioni della cartella di lavoro e imposta la proprietà HidePivotFieldList
            WorkbookSettings settings = workbook.Settings;
            settings.HidePivotFieldList = true; // Hide the pivot field list

            // Salva la cartella di lavoro
            workbook.Save("HidePivotFieldListDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


