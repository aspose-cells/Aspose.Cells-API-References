---
title: "Cell.SetDynamicArrayFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Establece una fórmula de matriz dinámica y hace que la fórmula se desborde a celdas vecinas si es posible"
type: docs
url: /es/net/aspose.cells/cell/setdynamicarrayformula/
---
## SetDynamicArrayFormula(string, FormulaParseOptions, bool) {#setdynamicarrayformula}

Establece una fórmula de matriz dinámica y hace que la fórmula se desborde a celdas vecinas si es posible.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    bool calculateValue)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arrayFormula | String | la expresión de la fórmula |
| opciones | FormulaParseOptions | opciones para analizar la fórmula. La opción "Parse" será ignorada y la fórmula siempre se analizará inmediatamente |
| calculateValue | Booleano | si calcular esta fórmula de matriz dinámica para esas celdas en el rango expandido. |

### Valor de retorno

el rango en el que la fórmula debe expandirse.

### Observaciones

el rango devuelto puede no ser el mismo que el real en el que esta fórmula de matriz dinámica se expande. Si hay celdas no vacías en el rango, la fórmula se establecerá solo para la celda actual y se marcará como "#SPILL!". Pero para este tipo de situación aún devolvemos todo el rango en el que esta fórmula debe expandirse.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsBooleDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Establecer fórmula de matriz dinámica en la celda A1
            Cell cell1 = cells["A1"];
            cell1.SetDynamicArrayFormula("=SEQUENCE(B2)", new FormulaParseOptions(), true);

            // Establecer valor en B2 que afectará la fórmula SEQUENCE
            cells["B2"].PutValue(3);

            // Calcular fórmulas y actualizar matrices dinámicas
            wb.CalculateFormula();
            wb.RefreshDynamicArrayFormulas(false);

            // Mostrar los resultados del rango expandido
            Console.WriteLine("Dynamic array results:");
            for (int i = 0; i < 3; i++)
            {
                Console.WriteLine(cells[0, i].Value);
            }
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDynamicArrayFormula(string, FormulaParseOptions, object[][], bool, bool) {#setdynamicarrayformula_1}

Establece una fórmula de matriz dinámica y hace que la fórmula se desborde a celdas vecinas si es posible.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    object[][] values, bool calculateRange, bool calculateValue)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arrayFormula | String | la expresión de la fórmula |
| opciones | FormulaParseOptions | opciones para analizar la fórmula. La opción "Parse" será ignorada y la fórmula siempre se analizará inmediatamente |
| values | Object[][] | valores (resultados calculados) para esas celdas con la fórmula de matriz dinámica dada |
| calculateRange | Booleano | Si calcular el rango expandido para esta fórmula de matriz dinámica. Si el parámetro "values" no es nulo y esta bandera es falsa, entonces la altura del rango expandido será values.Length y el ancho será values[0].Length. |
| calculateValue | Booleano | si calcular esta fórmula de matriz dinámica para esas celdas en el rango expandido cuando "values" es nulo o el elemento correspondiente en "values" para una celda es nulo. |

### Valor de retorno

el rango en el que la fórmula debe expandirse.

### Observaciones

el rango devuelto puede no ser el mismo que el real en el que esta fórmula de matriz dinámica se expande. Si hay celdas no vacías en el rango, la fórmula se establecerá solo para la celda actual y se marcará como "#SPILL!". Pero para este tipo de situación aún devolvemos todo el rango en el que esta fórmula debe expandirse.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            Cell cell = cells["A1"];
            cell.PutValue(10);
            cell = cells["A2"];
            cell.PutValue(20);
            cell = cells["B1"];
            cell.PutValue(60);
            cell = cells["B2"];
            cell.PutValue(80);

            // Obtener la celda C1 donde se establecerá la fórmula de matriz dinámica
            cell = worksheet.Cells["C1"];

            // Definir la fórmula de matriz dinámica
            string formula = "=A1:B2 * 2";
            
            // Crear opciones de análisis de fórmula
            FormulaParseOptions options = new FormulaParseOptions
            {
                Parse = true // Enable formula parsing
            };

            // Preparar valores para rellenar las celdas de resultados de la fórmula
            object[][] values = new object[2][];
            values[0] = new object[] { 2, 4 };
            values[1] = new object[] { 6, 8 };

            try
            {
                // Establecer fórmula de matriz dinámica con valores precalculados
                CellArea result = cell.SetDynamicArrayFormula(
                    formula,
                    options,
                    values,
                    calculateRange: false,  // Use values array dimensions for spill range
                    calculateValue: false  // Use provided values instead of calculating
                );

                Console.WriteLine($"Dynamic array formula set. Affected range: Rows {result.StartRow}-{result.EndRow}, Columns {result.StartColumn}-{result.EndColumn}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetDynamicArrayFormula: {ex.Message}");
            }

            // Guardar el libro de trabajo con los cambios
            workbook.Save("SetDynamicArrayFormulaDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDynamicArrayFormula(string, FormulaParseOptions, object[][], bool, bool, CalculationOptions) {#setdynamicarrayformula_2}

Establece una fórmula de matriz dinámica y hace que la fórmula se desborde a celdas vecinas si es posible.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    object[][] values, bool calculateRange, bool calculateValue, CalculationOptions copts)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arrayFormula | String | la expresión de la fórmula |
| opciones | FormulaParseOptions | opciones para analizar la fórmula. La opción "Parse" será ignorada y la fórmula siempre se analizará inmediatamente |
| values | Object[][] | valores (resultados calculados) para esas celdas con la fórmula de matriz dinámica dada |
| calculateRange | Booleano | Si calcular el rango expandido para esta fórmula de matriz dinámica. Si el parámetro "values" no es nulo y esta bandera es falsa, entonces la altura del rango expandido será values.Length y el ancho será values[0].Length. |
| calculateValue | Booleano | si calcular esta fórmula de matriz dinámica para esas celdas en el rango expandido cuando "values" es nulo o el elemento correspondiente en "values" para una celda es nulo. |
| copts | CalculationOptions | Las opciones para calcular la fórmula. Normalmente, por consideraciones de rendimiento, la propiedad [`Recursive`](../../calculationoptions/recursive/) debería ser false. |

### Valor de retorno

el rango en el que la fórmula debe expandirse.

### Observaciones

el rango devuelto puede no ser el mismo que el real en el que esta fórmula de matriz dinámica se expande. Si hay celdas no vacías en el rango, la fórmula se establecerá solo para la celda actual y se marcará como "#SPILL!". Pero para este tipo de situación aún devolvemos todo el rango en el que esta fórmula debe expandirse.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar datos de ejemplo en las celdas A2:B5
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(60);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B3"].PutValue(55);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["B5"].PutValue(70);

            // Obtener la celda objetivo D1
            Cell cellD1 = worksheet.Cells["D1"];

            try
            {
                // Preparar parámetros para SetDynamicArrayFormula
                string formula = "=FILTER(A2:A5, B2:B5>50)";
                FormulaParseOptions options = new FormulaParseOptions { Parse = true };
                object[][] values = new object[2][] { new object[] { 10 }, new object[] { 40 } };
                bool calculateRange = true;
                bool calculateValue = true;
                CalculationOptions calcOptions = new CalculationOptions { Recursive = true };

                // Llamar a SetDynamicArrayFormula con parámetros específicos
                CellArea spillRange = cellD1.SetDynamicArrayFormula(
                    formula,
                    options,
                    values,
                    calculateRange,
                    calculateValue,
                    calcOptions
                );

                Console.WriteLine($"Dynamic array formula set successfully. Spill range: {spillRange}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetDynamicArrayFormula method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("SetDynamicArrayFormulaDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


