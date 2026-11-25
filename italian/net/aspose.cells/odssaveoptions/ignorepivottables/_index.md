---
title: "OdsSaveOptions.IgnorePivotTables"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OdsSaveOptions. Indica se salvare le tabelle pivot"
type: docs
url: /it/net/aspose.cells/odssaveoptions/ignorepivottables/
---
## OdsSaveOptions.IgnorePivotTables property

Indica se salvare le tabelle pivot.

```csharp
public bool IgnorePivotTables { get; set; }
```

### Osservazioni

La funzionalità delle tabelle pivot di OpenOffice ha meno impostazioni rispetto a Excel, quindi i risultati delle tabelle pivot presentano molte differenze. A volte è meglio ignorare queste tabelle pivot durante il salvataggio del file .ods.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class OdsSaveOptionsPropertyIgnorePivotTablesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(3000);

            // Crea una tabella pivot
            PivotTableCollection pivotTables = workbook.Worksheets[0].PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Crea un'istanza di OdsSaveOptions
            OdsSaveOptions saveOptions = new OdsSaveOptions();

            // Visualizza il valore corrente di IgnorePivotTables
            Console.WriteLine("Current IgnorePivotTables value: " + saveOptions.IgnorePivotTables);

            // Imposta per ignorare le tabelle pivot durante il salvataggio
            saveOptions.IgnorePivotTables = true;

            // Salva con le tabelle pivot ignorate
            workbook.Save("IgnorePivotTablesDemo_Ignored.ods", saveOptions);

            // Imposta per includere le tabelle pivot durante il salvataggio
            saveOptions.IgnorePivotTables = false;

            // Salva con le tabelle pivot incluse
            workbook.Save("IgnorePivotTablesDemo_Included.ods", saveOptions);
        }
    }
}
```

### Vedi anche

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


