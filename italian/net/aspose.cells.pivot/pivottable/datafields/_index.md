---
title: "PivotTable.DataFields"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Ottiene una PivotFieldCollection che rappresenta tutti i campi dati in una PivotTable"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/datafields/
---
## PivotTable.DataFields property

Ottiene una [`PivotFieldCollection`](../../pivotfieldcollection/) che rappresenta tutti i campi dati in una PivotTable.

```csharp
public PivotFieldCollection DataFields { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataFieldsDemo
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
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;

            // Aggiungi una tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Aggiungi campo riga e campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Accedi ai campi dati e dimostra la funzionalità
            PivotFieldCollection dataFields = pivotTable.DataFields;
            if (dataFields.Count > 0)
            {
                PivotField dataField = dataFields[0];
                Console.WriteLine("Data Field Name: " + dataField.Name);
                Console.WriteLine("Data Field Function: " + dataField.Function);
            }

            // Salva la cartella di lavoro
            workbook.Save("PivotTableDataFieldsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


