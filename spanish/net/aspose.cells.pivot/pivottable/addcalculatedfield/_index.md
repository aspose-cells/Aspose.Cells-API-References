---
title: "PivotTable.AddCalculatedField"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de PivotTable. Añade un campo calculado al campo dinámico"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/addcalculatedfield/
---
## AddCalculatedField(string, string, bool) {#addcalculatedfield_1}

Agrega un campo calculado al campo dinámico.

```csharp
public void AddCalculatedField(string name, string formula, bool dragToDataArea)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre del campo calculado |
| fórmula | String | La fórmula del campo calculado. |
| dragToDataArea | Booleano | True, arrastra este campo al área de datos inmediatamente |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddCalculatedFieldWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "A";
            cells["B2"].Value = 100;
            cells["A3"].Value = "B";
            cells["B3"].Value = 150;
            cells["A4"].Value = "C";
            cells["B4"].Value = 200;

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Agregar campo calculado
            pivotTable.AddCalculatedField("DoubleSales", "=Sales*2", true);

            // Guarda el libro de trabajo
            workbook.Save("PivotTableWithCalculatedField.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddCalculatedField(string, string) {#addcalculatedfield}

Agrega un campo calculado al campo dinámico y lo arrastra al área de datos.

```csharp
public void AddCalculatedField(string name, string formula)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre del campo calculado |
| fórmula | String | La fórmula del campo calculado. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddCalculatedFieldWithStringStringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(8);
            
            worksheet.Cells["C1"].PutValue("Quantity");
            worksheet.Cells["C2"].PutValue(5);
            worksheet.Cells["C3"].PutValue(3);
            worksheet.Cells["C4"].PutValue(10);

            // Crear colección de tablas dinámicas
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Agregar tabla dinámica y obtener su índice
            int pivotIndex = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            
            // Obtener el objeto de tabla dinámica
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Agregar campos al área de filas
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Agregar campos de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Agregar campo calculado
            pivotTable.AddCalculatedField("Total", "=Price*Quantity");
            
            // Dar formato al campo de datos
            pivotTable.DataFields["Total"].NumberFormat = "$#,##0.00";
            
            // Actualizar y calcular la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableWithCalculatedField.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


