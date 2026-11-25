---
title: "TableStyleCollection.AddPivotTableStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo TableStyleCollection. Aggiunge uno stile pivot personalizzato"
type: docs
url: /it/net/aspose.cells.tables/tablestylecollection/addpivottablestyle/
---
## TableStyleCollection.AddPivotTableStyle method

Aggiunge uno stile personalizzato per tabella pivot.

```csharp
public int AddPivotTableStyle(string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome dello stile della tabella pivot. |

### Valore di ritorno

L'indice dello stile della tabella pivot.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleCollectionMethodAddPivotTableStyleWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Desktop");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(800);
            worksheet.Cells["A4"].PutValue("Tablet");
            worksheet.Cells["B4"].PutValue("East");
            worksheet.Cells["C4"].PutValue(500);

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, 1);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 2);

            try
            {
                // Ottieni la raccolta di stili della tabella
                TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

                // Chiama AddPivotTableStyle con parametro String
                int styleIndex = tableStyles.AddPivotTableStyle("CustomPivotStyle1");
                Console.WriteLine($"Added pivot table style at index: {styleIndex}");

                // Imposta il nuovo stile come stile pivot predefinito
                tableStyles.DefaultPivotStyleName = "CustomPivotStyle1";

                // Applica lo stile alla nostra tabella pivot
                pivotTable.PivotTableStyleName = "CustomPivotStyle1";
                Console.WriteLine("Applied custom pivot table style successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddPivotTableStyle method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("TableStyleCollectionMethodAddPivotTableStyleWithStringDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


