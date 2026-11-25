---
title: "PivotTable.PageFields"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Restituisce una PivotFieldCollection che è attualmente mostrata come campi di pagina"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/pagefields/
---
## PivotTable.PageFields property

Restituisce una [`PivotFieldCollection`](../../pivotfieldcollection/) che è attualmente mostrata come campi di pagina.

```csharp
public PivotFieldCollection PageFields { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPageFieldsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            var cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "P1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "P2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            
            cells["A4"].Value = "P3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 3000;
            
            cells["A5"].Value = "P1";
            cells["B5"].Value = "West";
            cells["C5"].Value = 4000;

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Aggiungi campi
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Region");

            // Accedi ai campi di pagina
            PivotFieldCollection pageFields = pivotTable.PageFields;
            
            Console.WriteLine("Page Fields:");
            foreach (PivotField field in pageFields)
            {
                Console.WriteLine($"Field: {field.Name}");
                Console.WriteLine("Items:");
                foreach (PivotItem item in field.PivotItems)
                {
                    Console.WriteLine($"- {item.Name} (Hidden: {item.IsHidden})");
                }
            }

            // Salva la cartella di lavoro
            workbook.Save("PivotTablePageFieldsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


