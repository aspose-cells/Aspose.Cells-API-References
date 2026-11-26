---
title: "Worksheet.AutoFitRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Worksheet. Ajusta automáticamente la altura de la fila en un rango rectangular"
type: docs
url: /es/net/aspose.cells/worksheet/autofitrow/
---
## AutoFitRow(int, int, int, int) {#autofitrow_3}

Ajusta automáticamente la altura de la fila en un rango rectangular.

```csharp
public void AutoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | Índice de fila inicial. |
| endRow | Int32 | Índice de fila final. |
| startColumn | Int32 | Índice de columna inicial. |
| endColumn | Int32 | Índice de columna final. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitRowWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            RowCollection rows = worksheet.Cells.Rows;
            rows[0].Height = 20;
            rows[1].Height = 20;
            // Agregar datos de ejemplo a las celdas para demostrar el ajuste automático de filas
            worksheet.Cells["A1"].PutValue("This is a long text that will demonstrate row autofit");
            worksheet.Cells["B1"].PutValue("Additional column with text");
            worksheet.Cells["A2"].PutValue("Shorter text");
            worksheet.Cells["B2"].PutValue("More text");
            
            try
            {
                Console.WriteLine($"Row 1 height before autofit: {worksheet.Cells.Rows[0].Height}");
                Console.WriteLine($"Row 2 height before autofit: {worksheet.Cells.Rows[1].Height}");

                // Llamar a AutoFitRow con los parámetros: startRow, endRow, startColumn, endColumn
                worksheet.AutoFitRow(0, 1, 0, 1);
                
                Console.WriteLine("AutoFitRow method executed successfully with parameters (0, 1, 0, 1)");
                
                // Mostrar el efecto mostrando las alturas de las filas
                Console.WriteLine($"Row 1 height after autofit: {worksheet.Cells.Rows[0].Height}");
                Console.WriteLine($"Row 2 height after autofit: {worksheet.Cells.Rows[1].Height}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitRow method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("AutoFitRowWithInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int) {#autofitrow}

Ajusta automáticamente la altura de la fila.

```csharp
public void AutoFitRow(int rowIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | Int32 | Índice de fila. |

### Observaciones

AutoFitRow es una función imprecisa.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowWithInt32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer texto largo con ajuste de texto en la celda A1
            worksheet.Cells["A1"].Value = "LOOOOOOOOOOOOOOOOOONG TEEEEEEEEEEXT";
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            // Ajustar automáticamente la primera fila
            worksheet.AutoFitRow(0);

            // Guarda el libro de trabajo
            workbook.Save("AutoFitRowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int, int, int) {#autofitrow_1}

Ajusta automáticamente la altura de la fila.

```csharp
public void AutoFitRow(int rowIndex, int firstColumn, int lastColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | Int32 | Índice de fila. |
| firstColumn | Int32 | Índice de primera columna. |
| lastColumn | Int32 | Índice de última columna. |

### Observaciones

Este método ajusta automáticamente una fila según el contenido en un rango de celdas dentro de la fila.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo a las celdas que afectarán la altura de la fila
            worksheet.Cells["A2"].PutValue("This is a long text that will demonstrate AutoFitRow functionality");
            worksheet.Cells["B2"].PutValue("Additional text in another column");
            
            // Ajustar automáticamente la fila (fila 2) entre las columnas 0 y 1 (A a B)
            worksheet.AutoFitRow(1, 0, 1);
            
            // Guarda el libro de trabajo
            workbook.Save("AutoFitRowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int, int, int, AutoFitterOptions) {#autofitrow_2}

Ajusta automáticamente la altura de la fila.

```csharp
public void AutoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | Int32 | Índice de fila. |
| firstColumn | Int32 | Índice de primera columna. |
| lastColumn | Int32 | Índice de última columna. |
| opciones | AutoFitterOptions | Las opciones del autoajustador |

### Observaciones

Este método ajusta automáticamente una fila según el contenido en un rango de celdas dentro de la fila.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowWithInt32Int32Int32AutoFitterOptioDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("This is a test string for autofit");
            worksheet.Cells["B1"].PutValue("Another test string in column B");
            
            // Crear AutoFitterOptions
            AutoFitterOptions options = new AutoFitterOptions
            {
                AutoFitMergedCells = true,
                IgnoreHidden = false,
                OnlyAuto = false
            };

            // Obtener la altura original de la fila
            double originalHeight = worksheet.Cells.GetRowHeight(0);
            Console.WriteLine($"Original row height: {originalHeight}");

            // Ajustar automáticamente la primera fila
            worksheet.AutoFitRow(0, 0, 2, options);

            // Obtener nueva altura de fila
            double newHeight = worksheet.Cells.GetRowHeight(0);
            Console.WriteLine($"New row height after AutoFit: {newHeight}");

            // Guarda el libro de trabajo
            workbook.Save("AutoFitRowExample.xlsx");
        }
    }
}
```

### Ver también

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


