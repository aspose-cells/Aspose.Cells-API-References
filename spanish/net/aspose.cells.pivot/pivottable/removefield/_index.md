---
title: "PivotTable.RemoveField"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotTable. Elimina un campo de un área de campo específica"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/removefield/
---
## RemoveField(PivotFieldType, string) {#removefield_2}

Elimina un campo de un área de campo específica

```csharp
public void RemoveField(PivotFieldType fieldType, string fieldName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldType | PivotFieldType | El tipo de área de los campos. |
| fieldName | String | El nombre en los campos base. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRemoveFieldWithPivotFieldTypeStringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("example.xlsx");
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accede a la primera tabla dinámica
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Eliminar el campo "c" del área de Datos
            pivotTable.RemoveField(PivotFieldType.Data, "c");
            
            // Calcular datos de tabla dinámica
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveField(PivotFieldType, int) {#removefield_1}

Elimina un campo de una región de tabla dinámica específica.

```csharp
public void RemoveField(PivotFieldType fieldType, int baseFieldIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldType | PivotFieldType | El tipo de área de los campos. |
| baseFieldIndex | Int32 | El índice del campo en los campos base. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodRemoveFieldWithPivotFieldTypeInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                // Eliminar el campo de fila (índice 0) de la tabla dinámica
                pivotTable.RemoveField(PivotFieldType.Row, 0);
                
                Console.WriteLine("Row field removed successfully from the pivot table");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveField method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("PivotTableRemoveFieldDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveField(PivotFieldType, PivotField) {#removefield}

Eliminar campo del área de campo específica

```csharp
public void RemoveField(PivotFieldType fieldType, PivotField pivotField)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldType | PivotFieldType | el tipo de área de campos. |
| pivotField | PivotField | el campo en los campos base. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRemoveFieldWithPivotFieldTypePivotFieldDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("TestFile.xlsx");
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accede a la primera tabla dinámica
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Eliminar un campo de columna de la tabla dinámica
            if (pivotTable.ColumnFields.Count > 0)
            {
                pivotTable.RemoveField(PivotFieldType.Column, pivotTable.ColumnFields[0]);
            }
            
            // Eliminar un campo de datos de la tabla dinámica
            if (pivotTable.DataFields.Count > 0)
            {
                pivotTable.RemoveField(PivotFieldType.Data, pivotTable.DataFields[0]);
            }
            
            // Guarda el libro de trabajo
            workbook.Save("ModifiedPivotTable.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


