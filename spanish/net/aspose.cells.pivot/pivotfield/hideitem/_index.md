---
title: "PivotField.HideItem"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotField. Establece si el PivotItem específico en un campo de datos está oculto"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/hideitem/
---
## HideItem(int, bool) {#hideitem}

Establece si el PivotItem específico en un campo de datos está oculto.

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideItem(int index, bool isHidden)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | el índice del pivotItem en el pivotField. |
| isHidden | Booleano | si el PivotItem específico está oculto |

### Observaciones

NOTA: Este método está obsoleto. En su lugar, utilice la propiedad PivotField.PivotItems[int].IsHidden. Este método será eliminado 12 meses después, a partir de agosto de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideItemWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con una tabla dinámica de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Datos de muestra para la tabla dinámica
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("PO-23-05");
            sheet.Cells["A3"].PutValue("PO-23-06");
            sheet.Cells["A4"].PutValue("PO-23-05");
            sheet.Cells["A5"].PutValue("PO-23-07");
            
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(1500);
            sheet.Cells["B5"].PutValue(3000);

            // Crear tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Obtener el campo de pivote
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Ocultar elementos que no sean "PO-23-05"
            for (int i = 0; i < pivotField.ItemCount; i++)
            {
                pivotField.HideItem(i, pivotField.Items[i] != "PO-23-05");
            }
            
            // Calcular tabla dinámica
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFieldHideItemDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## HideItem(string, bool) {#hideitem_1}

Establece si el PivotItem específico en un campo de datos está oculto.

```csharp
[Obsolete("Use PivotField.PivotItems[string].IsHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideItem(string itemValue, bool isHidden)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| itemValue | String | El nombre del pivotItem en el pivotField. |
| isHidden | Booleano | Indica si el PivotItem específico está oculto |

### Observaciones

NOTA: Este método está obsoleto. En su lugar, utilice la propiedad PivotField.PivotItems[string].IsHidden. Este método será eliminado 12 meses después, a partir de agosto de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodHideItemWithStringBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;
            worksheet.Cells["B5"].Value = 5;

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Obtener el campo de pivote
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Llame al método HideItem con los parámetros (String, Boolean)
                pivotField.HideItem("Apple", true);

                Console.WriteLine("Method executed successfully with parameters (String, Boolean)");
                Console.WriteLine("Apple items are now hidden in the pivot table");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing HideItem method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("PivotFieldMethodHideItemWithStringBooleanDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


