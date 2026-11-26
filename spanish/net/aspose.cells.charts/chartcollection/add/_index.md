---
title: "ChartCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ChartCollection. Agrega un gráfico a la colección"
type: docs
url: /es/net/aspose.cells.charts/chartcollection/add/
---
## Add(ChartType, int, int, int, int) {#add}

Añade un gráfico a la colección.

```csharp
public int Add(ChartType type, int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | ChartType | Tipo de gráfico |
| topRow | Int32 | Índice de fila superior izquierda. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| bottomRow | Int32 | Índice de fila inferior derecha |
| rightColumn | Int32 | Índice de columna inferior derecha |

### Valor de retorno

[`Chart`](../../chart/) object index.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodAddWithChartTypeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 1; i <= 10; i++)
            {
                sheet.Cells["A" + (i + 1)].PutValue("Cat " + i);
                sheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // Agregar un gráfico usando los parámetros especificados
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 2, 25, 11);
            Chart chart = sheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("=Sheet1!$A$1:$B$11", true);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(ChartType, string, int, int, int, int) {#add_2}

Añade un gráfico a la colección.

```csharp
[Obsolete("Use ChartCollection.Add(ChartType, string, bool ,int , int, int, int ) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(ChartType type, string dataRange, int topRow, int leftColumn, int rightRow, 
    int bottomColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | ChartType | Tipo de gráfico |
| dataRange | String | Especifica el rango de datos del gráfico |
| topRow | Int32 | Índice de fila superior izquierda. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| rightRow | Int32 | Índice de fila inferior derecha |
| bottomColumn | Int32 | Índice de columna inferior derecha |

### Valor de retorno

[`Chart`](../../chart/) object index.

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad `Add`. Esta propiedad será eliminada 12 meses después desde mayo de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionMethodAddWithChartTypeStringInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            try
            {
                // Llame al método Add con los parámetros (ChartType, String, Int32, Int32, Int32, Int32)
                int chartIndex = worksheet.Charts.Add(
                    ChartType.Column,          // Chart type
                    "A1:B4",                  // Data range
                    0,                        // Top row position
                    3,                        // Left column position
                    15,                       // Bottom row position
                    8                         // Right column position
                );

                Console.WriteLine("Chart added successfully at index: " + chartIndex);
                
                // Acceda al gráfico recién creado
                Chart chart = worksheet.Charts[chartIndex];
                chart.Title.Text = "Sample Column Chart";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("ChartCollectionMethodAddDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(byte[], string, bool, int, int, int, int) {#add_3}

Añade un gráfico con una plantilla predefinida.

```csharp
public int Add(byte[] data, string dataRange, bool isVertical, int topRow, int leftColumn, 
    int rightRow, int bottomColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| datos | Byte[] | Los datos del archivo de plantilla de gráfico (.crtx). |
| dataRange | String | Especifica el rango de datos del gráfico |
| isVertical | Booleano | Especifica si se debe trazar la serie a partir de un rango de valores de celdas por fila o por columna. |
| topRow | Int32 | Índice de fila superior izquierda. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| rightRow | Int32 | Índice de fila inferior derecha |
| bottomColumn | Int32 | Índice de columna inferior derecha |

### Valor de retorno

[`Chart`](../../chart/) object index.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionMethodAddWithByteArrayStringBooleanInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Cree una matriz de bytes que represente los datos del gráfico (ejemplo simplificado)
            byte[] chartData = new byte[] { 0x01, 0x02, 0x03 };

            try
            {
                // Llame al método Add con parámetros específicos
                int chartIndex = worksheet.Charts.Add(
                    chartData,          // Byte[] data
                    "A1:B4",            // String dataRange
                    true,               // Boolean isVertical
                    0,                  // Int32 topRow
                    0,                  // Int32 leftColumn
                    15,                 // Int32 rightRow
                    8                   // Int32 bottomColumn
                );

                Console.WriteLine($"Chart added successfully at index: {chartIndex}");

                // Acceda al gráfico agregado
                Chart chart = worksheet.Charts[chartIndex];
                chart.Type = ChartType.Column;

                // Guardar el resultado
                workbook.Save("ChartCollectionMethodAddDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(ChartType, string, bool, int, int, int, int) {#add_1}

Añade un gráfico a la colección.

```csharp
public int Add(ChartType type, string dataRange, bool isVertical, int topRow, int leftColumn, 
    int rightRow, int bottomColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | ChartType | Tipo de gráfico |
| dataRange | String | Especifica el rango de datos del gráfico |
| isVertical | Booleano | Especifica si se debe trazar la serie a partir de un rango de valores de celdas por fila o por columna. |
| topRow | Int32 | Índice de fila superior izquierda. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| rightRow | Int32 | Índice de fila inferior derecha |
| bottomColumn | Int32 | Índice de columna inferior derecha |

### Valor de retorno

[`Chart`](../../chart/) object index.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodAddWithChartTypeStringBooleanInt32IntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["C3"].PutValue(40);

            // Agregar gráfico con los parámetros especificados
            int chartIndex = worksheet.Charts.Add(ChartType.Column, "A1:C3", true, 4, 4, 14, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


