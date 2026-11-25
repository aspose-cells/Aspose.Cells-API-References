---
title: "OdsLoadOptions.RefreshPivotTables"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OdsLoadOptions. Indica se aggiornare le tabelle pivot durante il caricamento del file"
type: docs
url: /it/net/aspose.cells/odsloadoptions/refreshpivottables/
---
## OdsLoadOptions.RefreshPivotTables property

Indica se aggiornare le tabelle pivot durante il caricamento del file.

```csharp
public bool RefreshPivotTables { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class OdsLoadOptionsPropertyRefreshPivotTablesDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio con una tabella pivot
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Fruit");
            sheet.Cells["A4"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Item");
            sheet.Cells["B2"].PutValue("Apple");
            sheet.Cells["B3"].PutValue("Orange");
            sheet.Cells["B4"].PutValue("Carrot");
            sheet.Cells["C1"].PutValue("Price");
            sheet.Cells["C2"].PutValue(2.5);
            sheet.Cells["C3"].PutValue(3.0);
            sheet.Cells["C4"].PutValue(1.5);

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");

            // Salva come ODS
            string odsPath = "output.ods";
            wb.Save(odsPath, SaveFormat.Ods);

            // Carica con RefreshPivotTables abilitato
            OdsLoadOptions loadOptions = new OdsLoadOptions();
            loadOptions.RefreshPivotTables = true;
            Workbook wb2 = new Workbook(odsPath, loadOptions);

            // Verifica che la tabella pivot sia stata aggiornata
            Console.WriteLine("Pivot table count: " + wb2.Worksheets[0].PivotTables.Count);
        }
    }
}
```

### Vedi anche

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


