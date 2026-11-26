---
title: "Worksheet.CalculateArrayFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Worksheet. Calcula una fórmula como fórmula de matriz"
type: docs
url: /es/net/aspose.cells/worksheet/calculatearrayformula/
---
## CalculateArrayFormula(string, CalculationOptions) {#calculatearrayformula}

Calcula una fórmula como fórmula de matriz.

```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fórmula | String | Fórmula a calcular. |
| opciones | CalculationOptions | Opciones para calcular la fórmula |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateArrayFormulaWithStringCalculationOptionsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Poblar algunos datos de muestra
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(6);

            // Definir una fórmula de matriz
            string arrayFormula = "=SUM(A1:B3)";
            
            // Calcular la fórmula de matriz con opciones de cálculo
            object[][] result = worksheet.CalculateArrayFormula(arrayFormula, new CalculationOptions());
            
            // Mostrar el resultado
            Console.WriteLine("Result of array formula calculation: " + result[0][0]);
        }
    }
}
```

### Ver también

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateArrayFormula(string, CalculationOptions, int, int) {#calculatearrayformula_1}

Calcula una fórmula como fórmula de matriz.

```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts, int maxRowCount, 
    int maxColumnCount)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fórmula | String | Fórmula a calcular. |
| opciones | CalculationOptions | Opciones para calcular la fórmula |
| maxRowCount | Int32 | el recuento máximo de filas de los datos resultantes. Si es no positivo o mayor que el recuento real de filas, se usará el recuento real de filas. |
| maxColumnCount | Int32 | el recuento máximo de columnas de los datos resultantes. Si es no positivo o mayor que el recuento real de filas, entonces se usará el recuento real de columnas. |

### Valor de retorno

Resultado de la fórmula calculada.

### Observaciones

La fórmula se tomará como una fórmula de matriz dinámica para calcular la dimensión y el resultado. La dimensión máxima especificada por el usuario se utiliza en casos en que el resultado calculado es un conjunto de datos grande (por ejemplo, el resultado calculado puede corresponder a una fila o columna completa) pero el usuario no necesita una matriz tan grande según los requisitos del negocio o por consideraciones de rendimiento.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateArrayFormulaWithStringCalculationOptionsInt32IDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo y acceder a la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ejemplo 1: Cálculo simple de fórmula de matriz
            string formula = "=ISBLANK(IF(TRUE,B2:B5))";
            CalculationOptions options = new CalculationOptions();
            object[][] result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of ISBLANK(IF(TRUE,B2:B5)): " + result[0][0]);

            // Ejemplo 2: Fórmula de matriz con rango dinámico
            formula = "=LEN(IF({1;2;3;4},B2:B5))";
            result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of LEN(IF({1;2;3;4},B2:B5)): " + result[0][0]);

            // Ejemplo 3: Fórmula de matriz con la función MATCH
            // Configurar algunos datos de prueba
            sheet.Cells["B2"].PutValue(5);
            sheet.Cells["B3"].PutValue(10);
            sheet.Cells["C2"].PutValue(1);
            sheet.Cells["C3"].PutValue(2);
            sheet.Cells["D2"].PutValue(0);
            sheet.Cells["D3"].PutValue(0);

            formula = "=MATCH(1,IF(B2:B5=5,C2:C5,D2:D5),0)";
            result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of MATCH formula: " + result[0][0]);
        }
    }
}
```

### Ver también

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateArrayFormula(string, FormulaParseOptions, CalculationOptions, int, int, int, int, CalculationData) {#calculatearrayformula_2}

Calcula una fórmula como fórmula de matriz.

```csharp
public object[][] CalculateArrayFormula(string formula, FormulaParseOptions pOpts, 
    CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, 
    int maxColumnCount, CalculationData calculationData)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fórmula | String | Fórmula a calcular. |
| pOpts | FormulaParseOptions | Opciones para analizar la fórmula |
| cOpts | CalculationOptions | Opciones para calcular la fórmula |
| baseCellRow | Int32 | El índice de fila de la celda base. |
| baseCellColumn | Int32 | El índice de columna de la celda base. |
| maxRowCount | Int32 | El recuento máximo de filas de los datos resultantes. Si es no positivo o mayor que el recuento real de filas, se usará el recuento real de filas. |
| maxColumnCount | Int32 | El recuento máximo de columnas de los datos resultantes. Si es no positivo o mayor que el recuento real de filas, se usará el recuento real de columnas. |
| calculationData | CalculationData | Los datos de cálculo. Se utilizan para la situación en la que el usuario necesita calcular algunas fórmulas estáticas al implementar un motor de cálculo personalizado. Para este tipo de situación, el usuario debe especificarlos con los datos de cálculo proporcionados para [`Calculate`](../../abstractcalculationengine/calculate/). |

### Valor de retorno

Resultado de la fórmula calculada.

### Observaciones

La fórmula se tomará como una fórmula de matriz dinámica para calcular la dimensión y el resultado. La dimensión máxima especificada por el usuario se utiliza en casos en que el resultado calculado es un conjunto de datos grande (por ejemplo, el resultado calculado puede corresponder a una fila o columna completa) pero el usuario no necesita una matriz tan grande según los requisitos del negocio o por consideraciones de rendimiento.

### Ver también

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [CalculationData](../../calculationdata/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


