---
title: "PivotTable.ShowPivotStyleRowStripes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se la formattazione a righe a strisce è applicata"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/showpivotstylerowstripes/
---
## PivotTable.ShowPivotStyleRowStripes property

Indica se la formattazione a strisce per le righe è applicata.

```csharp
public bool ShowPivotStyleRowStripes { get; set; }
```

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowPivotStyleRowStripesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio
            DataTable data = new DataTable();
            data.Columns.Add("Category", typeof(string));
            data.Columns.Add("Product", typeof(string));
            data.Columns.Add("Sales", typeof(int));

            data.Rows.Add("Electronics", "Laptop", 1200);
            data.Rows.Add("Electronics", "Phone", 800);
            data.Rows.Add("Clothing", "Shirt", 50);
            data.Rows.Add("Clothing", "Pants", 70);
            data.Rows.Add("Furniture", "Chair", 150);
            data.Rows.Add("Furniture", "Table", 300);

            // Importa dati nel foglio di lavoro
            worksheet.Cells.ImportData(data, 0, 0, new ImportTableOptions());

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:C7", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi righe e colonne
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales

            // Abilita le righe a strisce
            pivotTable.ShowPivotStyleRowStripes = true;

            // Calcola i dati
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotTableWithRowStripes.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


