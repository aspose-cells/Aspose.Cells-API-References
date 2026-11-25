---
title: "PivotFieldCollection.AddByBaseIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotFieldCollection. Aggiunge un oggetto PivotField al tipo specifico PivotFields"
type: docs
url: /it/net/aspose.cells.pivot/pivotfieldcollection/addbybaseindex/
---
## PivotFieldCollection.AddByBaseIndex method

Aggiunge un oggetto PivotField al tipo specifico PivotFields.

```csharp
public int AddByBaseIndex(int baseFieldIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| baseFieldIndex | Int32 | indice del campo nei PivotFields di base. |

### Valore di ritorno

L'indice dell'oggetto PivotField in questi PivotFields.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionMethodAddByBaseIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dati di esempio
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Year";
            worksheet.Cells["B2"].Value = 2022;
            worksheet.Cells["B3"].Value = 2023;
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["C2"].Value = 1000;
            worksheet.Cells["C3"].Value = 2000;

            // Crea tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:C3", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Aggiungi campi iniziali
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Aggiungi il campo Year all'area di riga usando AddByBaseIndex
            int newIndex = pivotTable.RowFields.AddByBaseIndex(1);
            Console.WriteLine("Added field at index: " + newIndex);

            workbook.Save("PivotFieldAddByBaseIndexDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


