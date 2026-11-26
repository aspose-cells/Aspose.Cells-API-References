---
title: "Name.GetRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Name. Obtiene el rango si este nombre hace referencia a un rango"
type: docs
url: /es/net/aspose.cells/name/getrange/
---
## GetRange() {#getrange}

Obtiene el rango si este nombre se refiere a un rango.

```csharp
public Range GetRange()
```

### Valor de retorno

El rango.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            
            // Crear un rango con nombre
            int index = workbook.Worksheets.Names.Add("MyRange");
            workbook.Worksheets.Names[index].RefersTo = "=Sheet1!A1:B3";
            Name namedRange = workbook.Worksheets.Names[index];
            
            // Demostrar el método GetRange
            Aspose.Cells.Range range = namedRange.GetRange();
            Console.WriteLine("Named Range Address: " + range.Address);
            Console.WriteLine("Worksheet Name: " + range.Worksheet.Name);
            
            // Modificar el rango
            foreach (Cell cell in range)
            {
                if (cell.Row == 0)
                {
                    cell.PutValue(cell.StringValue.ToUpper());
                }
            }
            
            // Guarda el libro de trabajo
            workbook.Save("NamedRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRange(bool) {#getrange_1}

Obtiene el rango si este nombre se refiere a un rango

```csharp
public Range GetRange(bool recalculate)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| recalcular | Booleano | si recalcularlo si este nombre ya ha sido calculado antes de esta invocación. |

### Valor de retorno

El rango.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeWithBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Rellene datos de ejemplo
            for (int i = 0; i < 4; i++)
            {
                cells[i, 1].PutValue(i); // Column B values: 0,1,2,3
            }

            // Crear un rango con nombre con fórmula
            int nameIndex = wb.Worksheets.Names.Add("testname");
            Name name = wb.Worksheets.Names[nameIndex];
            name.RefersTo = "IFERROR(Sheet1!$B$2:$B$4,-1)";

            // Usar el rango con nombre en fórmulas
            cells["C1"].Formula = "=testname";
            cells["D1"].Formula = "SUM(testname)";

            // Calcular fórmulas
            wb.CalculateFormula();

            // Obtener el rango usando GetRange(true)
            Aspose.Cells.Range namedRange = name.GetRange(true);
            Console.WriteLine($"Named range: FirstRow={namedRange.FirstRow}, FirstColumn={namedRange.FirstColumn}, " +
                $"RowCount={namedRange.RowCount}, ColumnCount={namedRange.ColumnCount}");

            // Crear un gráfico usando el rango con nombre
            int chartIndex = sheet.Charts.Add(ChartType.Column, 10, 1, 20, 5);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("testname", true);
            Console.WriteLine($"Chart data points count: {chart.NSeries[0].CountOfDataValues}");
        }
    }
}
```

### Ver también

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRange(int, int, int) {#getrange_2}

Obtiene el rango si este nombre se refiere a un rango. Si la referencia de este nombre no es absoluta, el rango puede ser diferente para distintas celdas.

```csharp
public Range GetRange(int sheetIndex, int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex | Int32 | El índice de hoja correspondiente. |
| fila | Int32 | El índice de fila correspondiente. |
| columna | Int32 | El índice de columna correspondiente |

### Valor de retorno

El rango.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Dairy");
            
            // Crear un rango con nombre usando la firma de método correcta
            int index = workbook.Worksheets.Names.Add("SubCat");
            workbook.Worksheets.Names["SubCat"].RefersTo = "=" + worksheet.Name + "!A2:A4";
            
            // Obtener rango usando GetRange con parámetros de fila, columna y recuento de filas
            Aspose.Cells.Range range = workbook.Worksheets.Names["SubCat"].GetRange(0, 0, 3);
            
            // Mostrar la referencia del rango
            Console.WriteLine("Range refers to: " + range.RefersTo);
        }
    }
}
```

### Ver también

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


