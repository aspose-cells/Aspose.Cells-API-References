---
title: "PivotTable.ShowPivotStyleColumnStripes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se la formattazione a strisce è applicata per la colonna"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/showpivotstylecolumnstripes/
---
## PivotTable.ShowPivotStyleColumnStripes property

Indica se la formattazione a strisce è applicata per la colonna.

```csharp
public bool ShowPivotStyleColumnStripes { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowPivotStyleColumnStripesDemo
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
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 12;
            
            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Configura la tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sum of Quantity
            
            // Abilita le strisce di colonna
            pivotTable.ShowPivotStyleColumnStripes = true;
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableColumnStripesDemo.xlsx");
            
            Console.WriteLine("Pivot table with column stripes created successfully.");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


