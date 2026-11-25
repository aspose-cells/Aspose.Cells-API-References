---
title: "PivotTable.ErrorString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Ottiene la stringa visualizzata nelle celle che contengono errori quando la proprietà DisplayErrorString è true. Il valore predefinito è una stringa vuota"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/errorstring/
---
## PivotTable.ErrorString property

Restituisce la stringa visualizzata nelle celle che contengono errori quando la proprietà DisplayErrorString è true. Il valore predefinito è una stringa vuota.

```csharp
public string ErrorString { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyErrorStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bike";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Car";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bike";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Car";
            cells["B5"].Value = 1800;

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Imposta la proprietà ErrorString
            pivotTable.ErrorString = "Custom Error";
            pivotTable.DisplayErrorString = true;

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Calcola i dati e aggiorna la tabella pivot
            pivotTable.CalculateData();
            pivotTable.RefreshData();

            // Salva la cartella di lavoro
            workbook.Save("PivotTableErrorStringDemo.xlsx");

            Console.WriteLine("PivotTable with ErrorString property set successfully.");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


