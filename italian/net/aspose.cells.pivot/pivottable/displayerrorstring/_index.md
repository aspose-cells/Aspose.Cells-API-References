---
title: "PivotTable.DisplayErrorString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se il report PivotTable visualizza una stringa personalizzata nelle celle che contengono errori"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/displayerrorstring/
---
## PivotTable.DisplayErrorString property

Indica se il report PivotTable visualizza una stringa personalizzata nelle celle che contengono errori.

```csharp
public bool DisplayErrorString { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDisplayErrorStringDemo
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
            cells["B5"].Value = 2500;

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Imposta la proprietà DisplayErrorString e dimostra il suo utilizzo
            pivotTable.DisplayErrorString = true;
            pivotTable.ErrorString = "Custom Error";

            // Calcola i dati per mostrare l'effetto
            pivotTable.CalculateData();

            Console.WriteLine("DisplayErrorString is set to: " + pivotTable.DisplayErrorString);
            Console.WriteLine("ErrorString is set to: " + pivotTable.ErrorString);

            // Salva la cartella di lavoro
            workbook.Save("PivotTablePropertyDisplayErrorStringDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


