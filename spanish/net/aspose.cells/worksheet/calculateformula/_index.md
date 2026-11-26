---
title: "Worksheet.CalculateFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Worksheet. Calcula una fórmula"
type: docs
url: /es/net/aspose.cells/worksheet/calculateformula/
---
## CalculateFormula(string) {#calculateformula}

Calcula una fórmula.

```csharp
public object CalculateFormula(string formula)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fórmula | String | Fórmula a calcular. |

### Valor de retorno

Resultado de la fórmula calculada.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            Worksheet sheet = wb.Worksheets[0];

            // Demuestra la conversión básica de números
            string formula = "=NUMBERVALUE(\"1.234\")";
            Console.WriteLine("NUMBERVALUE(\"1.234\") = " + sheet.CalculateFormula(formula));

            // Demuestra la conversión de moneda
            formula = "=NUMBERVALUE(\"$1,234.56\")";
            Console.WriteLine("NUMBERVALUE(\"$1,234.56\") = " + sheet.CalculateFormula(formula));

            // Demuestra la conversión de tiempo
            formula = "=NUMBERVALUE(\"0:25\")";
            Console.WriteLine("NUMBERVALUE(\"0:25\") = " + sheet.CalculateFormula(formula));

            // Demuestra la conversión de fecha
            formula = "=NUMBERVALUE(\"07/26/2023\")";
            Console.WriteLine("NUMBERVALUE(\"07/26/2023\") = " + sheet.CalculateFormula(formula));

            // Demuestra el caso de error
            formula = "=NUMBERVALUE(\"invalid\")";
            Console.WriteLine("NUMBERVALUE(\"invalid\") = " + sheet.CalculateFormula(formula));
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(string, CalculationOptions) {#calculateformula_1}

Calcula directamente una expresión de fórmula.

```csharp
public object CalculateFormula(string formula, CalculationOptions opts)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fórmula | String | Fórmula a calcular. |
| opciones | CalculationOptions | Opciones para calcular la fórmula |

### Valor de retorno

Resultado calculado de la fórmula dada. El objeto devuelto puede ser de los posibles tipos de [`Value`](../../cell/value/), o ReferredArea.

### Observaciones

La fórmula se calculará tal como se ha establecido en la celda A1. Y la fórmula se tomará como una fórmula normal. Si necesitas que la fórmula se calcule como una fórmula de matriz y obtener una matriz para el resultado calculado, por favor usa [`CalculateArrayFormula`](../calculatearrayformula/) en su lugar.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringCalculationOptionsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Poblar algunos datos de muestra
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Crea un motor de cálculo personalizado
            CustomEngine customEngine = new CustomEngine();
            
            // Calcular fórmula usando motor personalizado
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = customEngine
            };
            
            object result = worksheet.CalculateFormula("=SUM(A1:A3)", options);
            
            Console.WriteLine("Calculation result: " + result);
        }
    }

    public class CustomEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object value = data.GetParamValue(i);
                    if (value is double)
                    {
                        sum += (double)value;
                    }
                }
                data.CalculatedValue = sum;
            }
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

## CalculateFormula(string, FormulaParseOptions, CalculationOptions, int, int, CalculationData) {#calculateformula_2}

Calcula directamente una expresión de fórmula.

```csharp
public object CalculateFormula(string formula, FormulaParseOptions pOpts, CalculationOptions cOpts, 
    int baseCellRow, int baseCellColumn, CalculationData calculationData)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fórmula | String | Fórmula a calcular. |
| pOpts | FormulaParseOptions | Opciones para analizar la fórmula. |
| cOpts | CalculationOptions | Opciones para calcular la fórmula. |
| baseCellRow | Int32 | El índice de fila de la celda base. |
| baseCellColumn | Int32 | El índice de columna de la celda base. |
| calculationData | CalculationData | Los datos de cálculo. Se utilizan para la situación en la que el usuario necesita calcular algunas fórmulas estáticas al implementar un motor de cálculo personalizado. Para este tipo de situación, el usuario debe especificarlos con los datos de cálculo proporcionados para [`Calculate`](../../abstractcalculationengine/calculate/). |

### Valor de retorno

Resultado calculado de la fórmula dada. El objeto devuelto puede ser de los posibles tipos de [`Value`](../../cell/value/), o ReferredArea.

### Observaciones

La fórmula se calculará tal como se haya establecido en la celda base especificada. Y la fórmula se tomará como una fórmula normal. Si necesita que la fórmula se calcule como una fórmula de matriz y obtener una matriz con el resultado calculado, por favor use [`CalculateArrayFormula`](../calculatearrayformula/) en su lugar.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringFormulaParseOptCalculati169472Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Rellene datos de ejemplo
            worksheet.Cells["B1"].PutValue(5);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C1"].PutValue(2);
            worksheet.Cells["C2"].PutValue(4);

            // Definir opciones de cálculo
            CalculationOptions calculationOptions = new CalculationOptions();
            
            // Definir opciones de análisis de fórmula
            FormulaParseOptions formulaParseOptions = new FormulaParseOptions();
            
            // Calcular fórmula con todos los parámetros
            object result = worksheet.CalculateFormula(
                "=SUM(B1:B2, C1:C2)",  // formula
                formulaParseOptions,   // parse options
                calculationOptions,    // calculation options
                0,                     // base cell row
                0,                     // base cell column
                null                   // calculation data
            );

            // Mostrar el resultado
            Console.WriteLine("Calculation result: " + result);
        }
    }
}
```

### Ver también

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [CalculationData](../../calculationdata/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(CalculationOptions, bool) {#calculateformula_3}

Calcula todas las fórmulas en esta hoja de cálculo.

```csharp
public void CalculateFormula(CalculationOptions options, bool recursive)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opciones | CalculationOptions | Opciones de cálculo |
| recursivo | Booleano | True significa que si las celdas de la hoja de cálculo dependen de celdas de otras hojas, las celdas dependientes en esas otras hojas también se calcularán. False indica que todas las fórmulas en la hoja de cálculo han sido calculadas y los valores son correctos. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithCalculationOptionsBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer datos de muestra y fórmulas
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B1"].PutValue("=SUM(A1:A3)");
            
            // Crear opciones de cálculo
            CalculationOptions options = new CalculationOptions();
            options.Recursive = true;
            options.IgnoreError = false;
            
            // Calcular fórmula con opciones y forzar cálculo completo
            worksheet.CalculateFormula(options, true);
            
            // Mostrar el resultado calculado
            Console.WriteLine("Calculated value: " + worksheet.Cells["B1"].StringValue);
        }
    }
}
```

### Ver también

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


