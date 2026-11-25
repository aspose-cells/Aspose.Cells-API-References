---
title: "PivotTable.RowFields"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Restituisce una PivotFieldCollection che sono attualmente mostrati come campi di riga"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/rowfields/
---
## PivotTable.RowFields property

Restituisce una [`PivotFieldCollection`](../../pivotfieldcollection/) che è attualmente mostrata come campi di riga.

```csharp
public PivotFieldCollection RowFields { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRowFieldsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Bike";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Bike";
            cells["B3"].Value = "South";
            cells["C3"].Value = 800;
            
            cells["A4"].Value = "Car";
            cells["B4"].Value = "North";
            cells["C4"].Value = 1500;
            
            cells["A5"].Value = "Car";
            cells["B5"].Value = "South";
            cells["C5"].Value = 1200;

            // Crea tabella pivot
            int pivotIndex = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Aggiungi campi di riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Region");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Dimostra la proprietà RowFields
            Console.WriteLine("Row Fields Count: " + pivotTable.RowFields.Count);
            Console.WriteLine("First Row Field Name: " + pivotTable.RowFields[0].Name);
            Console.WriteLine("Second Row Field Name: " + pivotTable.RowFields[1].Name);
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableRowFieldsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


