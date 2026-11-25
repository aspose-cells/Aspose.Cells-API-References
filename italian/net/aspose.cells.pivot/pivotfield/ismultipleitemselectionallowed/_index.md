---
title: "PivotField.IsMultipleItemSelectionAllowed"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotField proprietà. Indica se è possibile selezionare più elementi nel campo della pagina. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed/
---
## PivotField.IsMultipleItemSelectionAllowed property

Indica se è possibile selezionare più elementi nel campo pagina. Il valore predefinito è false.

```csharp
public bool IsMultipleItemSelectionAllowed { get; set; }
```

### Osservazioni

Solo per i campi della pagina (filtro).

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsMultipleItemSelectionAllowedDemo
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
            
            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Aggiungi campi
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Accedi al campo della pagina e imposta la selezione multipla
            PivotField pageField = pivotTable.PageFields[0];
            pageField.IsMultipleItemSelectionAllowed = true;
            
            // Verifica che la proprietà sia stata impostata
            Console.WriteLine("IsMultipleItemSelectionAllowed: " + pageField.IsMultipleItemSelectionAllowed);
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFieldIsMultipleItemSelectionAllowedDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


