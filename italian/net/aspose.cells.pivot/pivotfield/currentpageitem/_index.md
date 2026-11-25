---
title: "PivotField.CurrentPageItem"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotField proprietà. Ottiene o imposta l'elemento di pagina attualmente visualizzato solo per questo campo pivot."
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/currentpageitem/
---
## PivotField.CurrentPageItem property

Ottiene o imposta l'elemento di pagina attualmente visualizzato per questo campo pivot (solo campo pagina).

```csharp
public short CurrentPageItem { get; set; }
```

### Osservazioni

Usa [`AllPageItemsIndex`](../../pivotitem/allpageitemsindex/) (0x7FFD) come valore sentinella per indicare "Seleziona tutto". Questo è un marcatore predefinito e non è un indice di elemento valido.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyCurrentPageItemDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Apple";
            worksheet.Cells["A5"].Value = "Orange";
            
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["B4"].Value = "North";
            worksheet.Cells["B5"].Value = "East";
            
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["C2"].Value = 1000;
            worksheet.Cells["C3"].Value = 2000;
            worksheet.Cells["C4"].Value = 1500;
            worksheet.Cells["C5"].Value = 3000;

            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Aggiungi campi
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Product");
            
            // Aggiorna i dati
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Ottieni i campi della pagina
            PivotFieldCollection pageFields = pivotTable.PageFields;
            
            // Visualizza gli elementi della pagina corrente
            Console.WriteLine("Initial CurrentPageItem: " + pageFields[0].CurrentPageItem);
            
            // Modifica l'elemento della pagina corrente
            pageFields[0].CurrentPageItem = 1; // Change to Banana
            Console.WriteLine("After Change CurrentPageItem: " + pageFields[0].CurrentPageItem);
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFieldCurrentPageItemDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


