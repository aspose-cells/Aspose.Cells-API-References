---
title: "PivotTable.RepeatItemsOnEachPrintedPage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se le didascalie degli elementi pivot nell'area delle righe sono ripetute su ogni pagina stampata per i campi pivot in forma tabellare"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/repeatitemsoneachprintedpage/
---
## PivotTable.RepeatItemsOnEachPrintedPage property

Indica se le didascalie degli elementi pivot nell'area righe sono ripetute su ogni pagina stampata per i campi pivot in forma tabellare.

```csharp
public bool RepeatItemsOnEachPrintedPage { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyRepeatItemsOnEachPrintedPageDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["A2"].PutValue("North");
            worksheet.Cells["A3"].PutValue("North");
            worksheet.Cells["A4"].PutValue("South");
            worksheet.Cells["A5"].PutValue("South");
            worksheet.Cells["B1"].PutValue("Product");
            worksheet.Cells["B2"].PutValue("Apples");
            worksheet.Cells["B3"].PutValue("Oranges");
            worksheet.Cells["B4"].PutValue("Apples");
            worksheet.Cells["B5"].PutValue("Oranges");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["C3"].PutValue(1500);
            worksheet.Cells["C4"].PutValue(2000);
            worksheet.Cells["C5"].PutValue(2500);

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi di riga e campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Imposta la configurazione della pagina per la stampa
            worksheet.PageSetup.PrintTitleRows = "$1:$1";
            worksheet.PageSetup.PrintArea = "A1:G20";
            worksheet.PageSetup.FitToPagesTall = 0;
            worksheet.PageSetup.FitToPagesWide = 1;

            // Visualizza il valore corrente di RepeatItemsOnEachPrintedPage
            Console.WriteLine("Current RepeatItemsOnEachPrintedPage value: " + pivotTable.RepeatItemsOnEachPrintedPage);

            // Abilita la ripetizione degli elementi su ogni pagina stampata
            pivotTable.RepeatItemsOnEachPrintedPage = true;
            Console.WriteLine("RepeatItemsOnEachPrintedPage set to: " + pivotTable.RepeatItemsOnEachPrintedPage);

            // Calcola i dati per popolare la tabella pivot
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotTableRepeatItemsOnEachPrintedPageDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


