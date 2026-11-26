---
title: "Worksheet.AutoFitColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Worksheet. Ajusta automáticamente el ancho de la columna"
type: docs
url: /es/net/aspose.cells/worksheet/autofitcolumn/
---
## AutoFitColumn(int, int, int) {#autofitcolumn_1}

Ajusta automáticamente el ancho de la columna.

```csharp
public void AutoFitColumn(int columnIndex, int firstRow, int lastRow)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | Int32 | Índice de columna. |
| firstRow | Int32 | Índice de la primera fila. |
| lastRow | Int32 | Índice de la última fila. |

### Observaciones

Este método ajusta automáticamente una fila según el contenido en un rango de celdas dentro de la fila.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitColumnWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Rellenar celdas con datos de ejemplo que requerirán ajuste del ancho de columna
            worksheet.Cells["A1"].PutValue("Short text");
            worksheet.Cells["A2"].PutValue("This is a much longer piece of text that will require column width adjustment");
            worksheet.Cells["A3"].PutValue("Another long text entry to demonstrate AutoFitColumn");
            
            try
            {

                Console.WriteLine($"Column width before: {worksheet.Cells.GetColumnWidth(0)}");
                // Llamar a AutoFitColumn en la columna A (índice 0) para las filas 0 a 2 (basado en cero)
                worksheet.AutoFitColumn(0, 0, 2);
                
                Console.WriteLine("AutoFitColumn method executed successfully on column A for rows 1-3");
                
                // Mostrar el efecto mostrando el ancho de la columna antes y después                
                Console.WriteLine($"Column width after: {worksheet.Cells.GetColumnWidth(0)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitColumn method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("AutoFitColumnWithInt32Int32Int32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumn(int) {#autofitcolumn}

Ajusta automáticamente el ancho de la columna.

```csharp
public void AutoFitColumn(int columnIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | Int32 | Índice de columna. |

### Observaciones

AutoFitColumn es una función imprecisa.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas en la columna 4 (índice base 0)
            worksheet.Cells["D1"].PutValue("This is a test");
            worksheet.Cells["D2"].PutValue("AutoFitColumn demonstration");
            worksheet.Cells["D3"].PutValue("Aspose.Cells for .NET");
            
            // Ajustar automáticamente la columna 4 (índice base 0)
            worksheet.AutoFitColumn(3);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


