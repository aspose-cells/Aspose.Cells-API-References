---
title: "PivotTable.Indent"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Specifica l'incremento di rientro per l'asse compatto e può essere usata per impostare il Layout del report in Forma compatta"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/indent/
---
## PivotTable.Indent property

Specifica l'incremento di rientro per l'asse compatto e può essere usato per impostare il Layout del report in Forma compatta.

```csharp
public int Indent { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIndentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Imposta la proprietà di rientro
            pivotTable.Indent = 3;
            Console.WriteLine("Pivot Table Indent: " + pivotTable.Indent);

            // Salva la cartella di lavoro
            workbook.Save("PivotTableIndentDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


