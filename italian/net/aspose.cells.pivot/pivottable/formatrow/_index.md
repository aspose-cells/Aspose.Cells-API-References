---
title: "PivotTable.FormatRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Formatta i dati della riga nell'area della tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/formatrow/
---
## PivotTable.FormatRow method

Formatta i dati della riga nell'area della pivottable.

```csharp
public void FormatRow(int row, Style style)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice di riga dell'oggetto Row |
| stile | Stile | Stile da formattare |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodFormatRowWithInt32StyleDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            
            // Dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Crea stile per la formattazione
            Style style = wb.CreateStyle();
            style.Custom = "0.00%";
            style.Font.Name = "Calibri";
            style.Font.Size = 11;
            
            // Trova e formatta le righe
            Cell cell = worksheet.Cells.Find("A", null);
            if (cell != null)
            {
                pivotTable.FormatRow(cell.Row, style);
            }
            
            cell = worksheet.Cells.Find("B", null);
            if (cell != null)
            {
                pivotTable.FormatRow(cell.Row, style);
            }
            
            // Salva la cartella di lavoro
            wb.Save("PivotTableFormatRowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


