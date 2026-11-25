---
title: "PivotTable.IsAutoFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se il report PivotTable è formattato automaticamente. Casella di controllo autoformattazione tabella che si trova nell'opzione pivottable per Excel 2003"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/isautoformat/
---
## PivotTable.IsAutoFormat property

Indica se il report PivotTable è formattato automaticamente. Casella di controllo "autoformat table" presente nelle opzioni PivotTable per Excel 2003.

```csharp
public bool IsAutoFormat { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsAutoFormatDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);

            // Aggiungi una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Configura la tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Imposta la proprietà IsAutoFormat
            pivotTable.IsAutoFormat = true; // Enable auto formatting
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotTableIsAutoFormatDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


