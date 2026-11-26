---
title: "PivotTable.ShowPivotStyleRowStripes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Indica si se aplica el formato de franjas de fila"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/showpivotstylerowstripes/
---
## PivotTable.ShowPivotStyleRowStripes property

Indica si se aplica formato de rayas en filas.

```csharp
public bool ShowPivotStyleRowStripes { get; set; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de ejemplo
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

            // Importar datos a la hoja de cálculo
            worksheet.Cells.ImportData(data, 0, 0, new ImportTableOptions());

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:C7", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar filas y columnas
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales

            // Habilitar franjas de fila
            pivotTable.ShowPivotStyleRowStripes = true;

            // Calcular datos
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotTableWithRowStripes.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


