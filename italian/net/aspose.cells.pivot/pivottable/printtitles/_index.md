---
title: "PivotTable.PrintTitles"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se i titoli di stampa per il foglio di lavoro sono impostati in base al report della PivotTable. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/printtitles/
---
## PivotTable.PrintTitles property

Indica se i titoli di stampa per il foglio di lavoro sono impostati in base al report della PivotTable. Il valore predefinito è false.

```csharp
public bool PrintTitles { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPrintTitlesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro e alcuni dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Configura i campi della tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Dimostra la proprietà PrintTitles
            pivotTable.PrintTitles = true;
            Console.WriteLine("PrintTitles set to: " + pivotTable.PrintTitles);

            // Salva la cartella di lavoro
            workbook.Save("PivotTablePrintTitlesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


