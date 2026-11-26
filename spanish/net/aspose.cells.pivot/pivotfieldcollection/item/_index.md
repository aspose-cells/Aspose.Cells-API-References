---
title: "PivotFieldCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotFieldCollection. Obtiene el objeto PivotField en el índice específico"
type: docs
url: /es/net/aspose.cells.pivot/pivotfieldcollection/item/
---
## PivotFieldCollection indexer (1 of 2)

Obtiene el objeto PivotField en el índice específico.

```csharp
public PivotField this[int index] { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo y obtener la primera hoja
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Agregar una tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Agregar campos a áreas
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Acceder al primer campo de fila usando la propiedad Item y establecer IsAutoSort
            pivotTable.RowFields[0].IsAutoSort = true;
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFieldCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotFieldCollection indexer (2 of 2)

Obtiene el objeto PivotField del nombre específico.

```csharp
public PivotField this[string name] { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            ws.Cells["A1"].Value = "Category";
            ws.Cells["B1"].Value = "Value";
            ws.Cells["A2"].Value = "A";
            ws.Cells["B2"].Value = 10;
            ws.Cells["A3"].Value = "B";
            ws.Cells["B3"].Value = 20;
            ws.Cells["A4"].Value = "A";
            ws.Cells["B4"].Value = 30;
            ws.Cells["A5"].Value = "B";
            ws.Cells["B5"].Value = 40;

            // Crear tabla dinámica
            int index = ws.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pTable = ws.PivotTables[index];
            
            // Agregar campos a la tabla dinámica
            pTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Demostrar el uso de la propiedad Item
            pTable.DataFields["Sum of Value"].IsAutoSort = true;
            pTable.DataFields["Sum of Value"].IsAscendSort = false;
            
            // Actualizar y calcular la tabla dinámica
            pTable.RefreshData();
            pTable.CalculateData();
            
            // Guarda el libro de trabajo
            wb.Save("PivotFieldCollectionPropertyItemDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


