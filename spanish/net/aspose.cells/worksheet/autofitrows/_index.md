---
title: "Worksheet.AutoFitRows"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Worksheet. Ajusta automáticamente todas las filas en esta hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/autofitrows/
---
## AutoFitRows(AutoFitterOptions) {#autofitrows_1}

Ajusta automáticamente todas las filas en esta hoja de cálculo.

```csharp
public void AutoFitRows(AutoFitterOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opciones | AutoFitterOptions | Las opciones del autoajustador |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer datos de muestra y formato
            worksheet.Cells["A1"].PutValue("This is a long text that will need auto-fitting");
            worksheet.Cells["A2"].PutValue("Another long text\nwith multiple lines\nfor demonstration");
            
            // Combinar celdas para demostrar el ajuste automático de celdas combinadas
            worksheet.Cells.Merge(3, 0, 2, 1);
            worksheet.Cells["A3"].PutValue("Merged cells text that needs to fit");

            // Ajustar filas automáticamente con opciones específicas
            worksheet.AutoFitRows(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                MaxRowHeight = 100,  // Set reasonable max height
                OnlyAuto = true
            });

            // Guarda el libro de trabajo
            workbook.Save("AutoFitRowsDemo.xlsx");
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

## AutoFitRows(int, int) {#autofitrows_3}

Ajusta automáticamente la altura de la fila en un rango.

```csharp
public void AutoFitRows(int startRow, int endRow)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | Índice de fila inicial. |
| endRow | Int32 | Índice de fila final. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Rellenar celdas con datos de muestra y estilos
            for (int i = 0; i <= 8; i++)
            {
                Cell cell = cells[i, i];
                cell.Value = "Sample text for row " + i;
                
                if (i % 2 == 0)
                {
                    Style style = cell.GetStyle();
                    style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, System.Drawing.Color.Black);
                    cell.SetStyle(style);
                }
            }

            // Ajustar automáticamente filas del índice 0 al 8
            sheet.AutoFitRows(0, 8);

            // Mostrar las alturas de fila resultantes
            for (int i = 0; i <= 8; i++)
            {
                Console.WriteLine($"Row {i} height: {cells.GetRowHeightPixel(i)} pixels");
            }
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(int, int, AutoFitterOptions) {#autofitrows_4}

Ajusta automáticamente la altura de la fila en un rango.

```csharp
public void AutoFitRows(int startRow, int endRow, AutoFitterOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | Índice de fila inicial. |
| endRow | Int32 | Índice de fila final. |
| opciones | AutoFitterOptions | Las opciones del ajustador automático. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithInt32Int32AutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("This is a test string for auto-fit row height demonstration");
            worksheet.Cells["A2"].PutValue("Another line\nwith multiple lines\nof text");
            
            // Crear opciones del ajustador automático
            AutoFitterOptions options = new AutoFitterOptions();
            options.OnlyAuto = true;
            
            // Ajustar filas 0 a 1 con opciones
            worksheet.AutoFitRows(0, 1, options);
            
            // Guarda el libro de trabajo
            workbook.Save("AutoFitRowsDemo.xlsx");
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

## AutoFitRows() {#autofitrows}

Ajusta automáticamente todas las filas en esta hoja de cálculo.

```csharp
public void AutoFitRows()
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("This is a test string for AutoFitRows demonstration");
            worksheet.Cells["A2"].PutValue("Another line of text\nwith line break to show row height adjustment");
            worksheet.Cells["B1"].PutValue("Column B content");
            
            // Ajustar automáticamente las filas
            worksheet.AutoFitRows();
            
            // Ajustar automáticamente las columnas para una mejor visibilidad
            worksheet.AutoFitColumns();
            
            // Guarda el libro de trabajo
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "AutoFitRowsDemo.xlsx");
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            Console.WriteLine("Worksheet with AutoFitRows saved to: " + outputPath);
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(bool) {#autofitrows_2}

Ajusta automáticamente todas las filas en esta hoja de cálculo.

```csharp
public void AutoFitRows(bool onlyAuto)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| onlyAuto | Booleano | True, solo ajusta automáticamente la altura de la fila cuando la altura de la fila no está personalizada. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar texto de muestra a las celdas para demostrar el ajuste automático de filas
            worksheet.Cells["A1"].PutValue("This is a sample text that will demonstrate AutoFitRows functionality");
            worksheet.Cells["A2"].PutValue("Another line of text\nwith line breaks\nto show multi-line row adjustment");
            
            // Ajustar filas automáticamente con consideración de auto-merge
            worksheet.AutoFitRows(true);
            
            // Guarda el libro de trabajo
            workbook.Save("AutoFitRowsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


