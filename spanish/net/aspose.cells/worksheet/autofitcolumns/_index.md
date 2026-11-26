---
title: "Worksheet.AutoFitColumns"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Worksheet. Ajusta automáticamente todas las columnas en esta hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/autofitcolumns/
---
## AutoFitColumns() {#autofitcolumns}

Ajusta automáticamente todas las columnas en esta hoja de cálculo.

```csharp
public void AutoFitColumns()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("This is a test string");
            worksheet.Cells["B1"].PutValue("Another longer test string for demonstration");
            worksheet.Cells["C1"].PutValue("Short");
            
            // Ajustar automáticamente todas las columnas en la hoja de cálculo
            worksheet.AutoFitColumns();
            
            // Guarda el libro de trabajo
            workbook.Save("AutoFitColumnsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(AutoFitterOptions) {#autofitcolumns_1}

Ajusta automáticamente todas las columnas en esta hoja de cálculo.

```csharp
public void AutoFitColumns(AutoFitterOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opciones | AutoFitterOptions | Las opciones de ajuste automático |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsWithAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Sample Text for AutoFit");
            worksheet.Cells["B1"].PutValue("Longer Sample Text for Testing AutoFitColumns");
            worksheet.Cells["C1"].PutValue(12345.6789);
            
            // Crear opciones del ajustador automático
            AutoFitterOptions options = new AutoFitterOptions();
            options.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
            
            // Ajustar columnas con opciones
            worksheet.AutoFitColumns(options);
            
            // Guarda el libro de trabajo
            workbook.Save("AutoFitColumnsWithOptions.xlsx");
        }
    }
}
```

### Ver también

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int) {#autofitcolumns_2}

Ajusta automáticamente el ancho de las columnas.

```csharp
public void AutoFitColumns(int firstColumn, int lastColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstColumn | Int32 | Índice de primera columna. |
| lastColumn | Int32 | Índice de última columna. |

### Observaciones

AutoFitColumn es una función imprecisa.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para demostrar el ajuste automático
            sheet.Cells["A1"].PutValue("Short");
            sheet.Cells["B1"].PutValue("Medium length text");
            sheet.Cells["C1"].PutValue("Very very long text that needs column width adjustment");
            sheet.Cells["D1"].PutValue("Another example with different length");

            // AutoFit columnas desde el índice 0 hasta 3
            sheet.AutoFitColumns(0, 3);

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

---

## AutoFitColumns(int, int, AutoFitterOptions) {#autofitcolumns_3}

Ajusta automáticamente el ancho de las columnas.

```csharp
public void AutoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstColumn | Int32 | Índice de primera columna. |
| lastColumn | Int32 | Índice de última columna. |
| opciones | AutoFitterOptions | Las opciones de ajuste automático |

### Observaciones

AutoFitColumn es una función imprecisa.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitColumnsWithInt32Int32AutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Short text");
            worksheet.Cells["B1"].PutValue("This is a much longer text that needs column autofitting");
            worksheet.Cells["C1"].PutValue("Another example with different length");

            // Crear AutoFitterOptions con configuraciones específicas
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;
            options.IgnoreHidden = false;
            options.OnlyAuto = false;

            try
            {
                // Llamar a AutoFitColumns con los parámetros (firstColumn, lastColumn, options)
                worksheet.AutoFitColumns(0, 2, options);
                
                Console.WriteLine("AutoFitColumns method executed successfully with parameters (Int32, Int32, AutoFitterOptions)");
                
                // Mostrar el efecto mostrando los anchos de columna
                Console.WriteLine($"Column A width: {worksheet.Cells.GetColumnWidth(0)}");
                Console.WriteLine($"Column B width: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine($"Column C width: {worksheet.Cells.GetColumnWidth(2)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitColumns method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("AutoFitColumnsWithOptionsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int, int, int) {#autofitcolumns_4}

Ajusta automáticamente el ancho de las columnas.

```csharp
public void AutoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | Int32 | Índice de la primera fila. |
| firstColumn | Int32 | Índice de primera columna. |
| lastRow | Int32 | Índice de la última fila. |
| lastColumn | Int32 | Índice de última columna. |

### Observaciones

AutoFitColumn es una función imprecisa.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Rellenar algunos datos para la demostración
            worksheet.Cells["A1"].PutValue("Short");
            worksheet.Cells["B1"].PutValue("Medium length text");
            worksheet.Cells["C1"].PutValue("Very very long text that needs more column width");
            
            // AutoFit columnas desde la columna 0 (A) hasta la columna 2 (C), con la primera fila 0 y la última fila 0
            worksheet.AutoFitColumns(0, 2, 0, 0);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int, int, int, AutoFitterOptions) {#autofitcolumns_5}

Ajusta automáticamente el ancho de las columnas.

```csharp
public void AutoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, 
    AutoFitterOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | Int32 | Índice de la primera fila. |
| firstColumn | Int32 | Índice de primera columna. |
| lastRow | Int32 | Índice de la última fila. |
| lastColumn | Int32 | Índice de última columna. |
| opciones | AutoFitterOptions | Las opciones de ajuste automático |

### Observaciones

AutoFitColumn es una función imprecisa.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitColumnsWithInt32Int32Int32Int32AutoFitterDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rellenar celdas con datos de ejemplo que requieren ajuste del ancho de columna
            worksheet.Cells["A1"].PutValue("This is a long text that needs column autofit");
            worksheet.Cells["B1"].PutValue("Another lengthy text string for demonstration");
            worksheet.Cells["C1"].PutValue("Short");
            worksheet.Cells["A2"].PutValue(12345.6789);
            worksheet.Cells["B2"].PutValue("Multi-line\ntext\nsample");
            worksheet.Cells["C2"].PutValue(true);

            // Crear AutoFitterOptions con configuraciones específicas
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;
            options.IgnoreHidden = false;
            options.OnlyAuto = false;

            try
            {
                // Llamar a AutoFitColumns con parámetros específicos (firstRow, firstColumn, lastRow, lastColumn, options)
                worksheet.AutoFitColumns(0, 0, 1, 2, options);
                
                Console.WriteLine("AutoFitColumns method executed successfully with parameters (Int32, Int32, Int32, Int32, AutoFitterOptions)");
                
                // Mostrar los anchos de columna después del ajuste automático
                Console.WriteLine($"Column A width after autofit: {worksheet.Cells.GetColumnWidth(0)}");
                Console.WriteLine($"Column B width after autofit: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine($"Column C width after autofit: {worksheet.Cells.GetColumnWidth(2)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitColumns method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("AutoFitColumnsWithOptionsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


