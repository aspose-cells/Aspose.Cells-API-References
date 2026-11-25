---
title: "PivotField.IsInsertPageBreaksBetweenItems"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Indica se inserire interruzioni di pagina dopo ogni elemento. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems/
---
## PivotField.IsInsertPageBreaksBetweenItems property

Indica se inserire interruzioni di pagina dopo ogni elemento. Il valore predefinito è false.

```csharp
public bool IsInsertPageBreaksBetweenItems { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsInsertPageBreaksBetweenItemsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 7; i++)
            {
                worksheet.Cells["A" + i].PutValue("Category " + (i % 3 + 1));
                worksheet.Cells["B" + i].PutValue(i * 100);
            }

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B7", "E3", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Verifica il conteggio delle pagine prima di impostare la proprietà
            SheetRender render1 = new SheetRender(worksheet, new ImageOrPrintOptions());
            Console.WriteLine("Page count before: " + render1.PageCount);

            // Imposta la proprietà IsInsertPageBreaksBetweenItems
            PivotField field = pivotTable.RowFields[0];
            field.IsInsertPageBreaksBetweenItems = true;
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Verifica il conteggio delle pagine dopo aver impostato la proprietà
            SheetRender render2 = new SheetRender(worksheet, new ImageOrPrintOptions());
            Console.WriteLine("Page count after: " + render2.PageCount);

            // Salva la cartella di lavoro
            workbook.Save("PivotFieldIsInsertPageBreaksBetweenItemsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


