---
title: "TableStyleCollection.AddPivotTableStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método TableStyleCollection. Agrega un estilo de tabla dinámica personalizado"
type: docs
url: /es/net/aspose.cells.tables/tablestylecollection/addpivottablestyle/
---
## TableStyleCollection.AddPivotTableStyle method

Agrega un estilo de tabla dinámica personalizado.

```csharp
public int AddPivotTableStyle(string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre del estilo de tabla dinámica. |

### Valor de retorno

El índice del estilo de tabla dinámica.

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
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

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, 1);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 2);

            try
            {
                // Obtener la colección de estilos de tabla
                TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

                // Llamar a AddPivotTableStyle con un parámetro String
                int styleIndex = tableStyles.AddPivotTableStyle("CustomPivotStyle1");
                Console.WriteLine($"Added pivot table style at index: {styleIndex}");

                // Establecer el nuevo estilo como estilo predeterminado de tabla dinámica
                tableStyles.DefaultPivotStyleName = "CustomPivotStyle1";

                // Aplicar el estilo a nuestra tabla dinámica
                pivotTable.PivotTableStyleName = "CustomPivotStyle1";
                Console.WriteLine("Applied custom pivot table style successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddPivotTableStyle method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("TableStyleCollectionMethodAddPivotTableStyleWithStringDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


