---
title: "PivotField.FilterByLabel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotField method. Filtra per didascalie del campo pivot di riga o colonna"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/filterbylabel/
---
## PivotField.FilterByLabel method

Filtra per didascalie del campo pivot di riga o colonna.

```csharp
public PivotFilter FilterByLabel(PivotFilterType type, string label1, string label2)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | PivotFilterType | Il tipo di dati di filtraggio. |
| label1 | String | L'etichetta della condizione di filtro |
| label2 | String | L'etichetta superiore della condizione di filtro tra |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterByLabelWithPivotFilterTypeStringStringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("");
            sheet.Cells["A5"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            sheet.Cells["B5"].PutValue(40);

            // Crea una tabella pivot con i parametri corretti
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            pivot.AddFieldToArea(PivotFieldType.Row, "Category");
            pivot.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Ottieni il campo pivot
            PivotField field = pivot.RowFields[0];
            
            // Applica i filtri
            field.FilterByLabel(PivotFilterType.CaptionNotEqual, "(blank)", "");
            pivot.RefreshData();
            pivot.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFilterByLabelDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


