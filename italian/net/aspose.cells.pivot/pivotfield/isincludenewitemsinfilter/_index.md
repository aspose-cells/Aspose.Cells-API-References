---
title: "PivotField.IsIncludeNewItemsInFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Indica se includere nuovi elementi nel campo nel filtro manuale. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/isincludenewitemsinfilter/
---
## PivotField.IsIncludeNewItemsInFilter property

Indica se includere nuovi elementi nel campo nel filtro manuale. Il valore predefinito è false.

```csharp
public bool IsIncludeNewItemsInFilter { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsIncludeNewItemsInFilterDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;

            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Ottieni il campo pivot e imposta IsIncludeNewItemsInFilter
            PivotField field = pivotTable.RowFields[0];
            field.IsIncludeNewItemsInFilter = true;
            
            // Restituisci il valore della proprietà
            Console.WriteLine("IsIncludeNewItemsInFilter: " + field.IsIncludeNewItemsInFilter);
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFieldPropertyIsIncludeNewItemsInFilterDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


