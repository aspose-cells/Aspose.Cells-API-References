---
title: "PivotTable.SaveData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se i dati per il report della PivotTable sono salvati con la cartella di lavoro"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/savedata/
---
## PivotTable.SaveData property

Indica se i dati del report della PivotTable sono salvati con la cartella di lavoro.

```csharp
public bool SaveData { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertySaveDataDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
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

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Configura la tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Dimostra la proprietà SaveData
            Console.WriteLine("SaveData before setting: " + pivotTable.SaveData);
            pivotTable.SaveData = false; // Disable saving pivot data with file
            Console.WriteLine("SaveData after setting: " + pivotTable.SaveData);
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTable_SaveData_Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


