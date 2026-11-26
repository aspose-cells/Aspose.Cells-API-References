---
title: "Cell.SetFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Establecer la fórmula y el valor calculado de la fórmula"
type: docs
url: /es/net/aspose.cells/cell/setformula/
---
## SetFormula(string, object) {#setformula_3}

Establece la fórmula y el valor (resultado calculado) de la fórmula.

```csharp
public void SetFormula(string formula, object value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fórmula | String | La fórmula. |
| valor | Objeto | El valor (resultado calculado) de la fórmula. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringObjectDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer fórmula con parámetros de cadena y objeto
            cells["A1"].SetFormula("=SUM(1,2)", 4); // Will display 4 until calculation
            cells["A2"].SetFormula("=AVERAGE(5,10)", 7.5); // Will display 7.5 until calculation

            // Mostrar valores antes del cálculo
            Console.WriteLine("Before Calculation:");
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("A2: " + cells["A2"].StringValue);

            // Calcular fórmulas
            workbook.CalculateFormula();

            // Mostrar valores después del cálculo
            Console.WriteLine("\nAfter Calculation:");
            Console.WriteLine("A1: " + cells["A1"].IntValue); // Should show 3
            Console.WriteLine("A2: " + cells["A2"].DoubleValue); // Should show 7.5
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, FormulaParseOptions) {#setformula}

Establece la fórmula y el valor (resultado calculado) de la fórmula.

```csharp
public void SetFormula(string formula, FormulaParseOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fórmula | String | La fórmula. |
| opciones | FormulaParseOptions | Opciones para analizar la fórmula. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringFormulaParseOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtener una celda específica (B2 en este caso)
            Cell cell = worksheet.Cells["B2"];
            
            // Establecer algunos valores iniciales para la demostración
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].PutValue(30);
            
            // Ejemplo 1: Establecer una fórmula simple con opciones de análisis predeterminadas
            cell.SetFormula("=SUM(A1:A2)", new FormulaParseOptions());
            Console.WriteLine("Formula with default options: " + cell.Formula);
            
            // Ejemplo 2: Establecer fórmula con estilo R1C1 usando FormulaParseOptions
            FormulaParseOptions options = new FormulaParseOptions();
            options.Parse = true;
            options.R1C1Style = true;
            
            cell.SetFormula("=SUM(R[-1]C[-1]:R[0]C[-1])", options);
            Console.WriteLine("Formula with R1C1 style: " + cell.Formula);
            
            // Ejemplo 3: Establecer fórmula con opciones de análisis que preservan el formato R1C1
            options = new FormulaParseOptions();
            options.Parse = true;
            options.R1C1Style = true;
            cell.SetFormula("=R1C1+R2C2", options);
            Console.WriteLine("Formula preserved as R1C1: " + cell.Formula);
            
            // Calcule el libro de trabajo para ver los resultados
            workbook.CalculateFormula();
            Console.WriteLine("Calculated value: " + cell.Value);
        }
    }
}
```

### Ver también

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, bool, bool, object) {#setformula_2}

Establezca la fórmula y el valor de la fórmula.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetFormula(string formula, bool isR1C1, bool isLocal, object value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fórmula | String | La fórmula. |
| isR1C1 | Booleano | Si la fórmula es una fórmula R1C1. |
| isLocal | Booleano | Si la fórmula está formateada según la configuración regional. |
| valor | Objeto | El valor de la fórmula. |

### Observaciones

NOTA: Esta clase ahora está obsoleta. En su lugar, utilice Cell.SetFormula(string,FormulaParseOptions,object). Esta propiedad será eliminada 12 meses después desde diciembre de 2019. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetFormulaWithStringBooleanBooleanObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].PutValue(30);
            worksheet.Cells["B2"].PutValue(40);

            // Obtenga la celda objetivo donde estableceremos la fórmula
            Cell cell = worksheet.Cells["C1"];

            try
            {
                // Establezca una fórmula con todos los parámetros
                // Parámetros: cadena de fórmula, isR1C1, isLocal, valor
                cell.SetFormula("=SUM(A1:B2)", false, false, null);

                // Calcular la fórmula
                workbook.CalculateFormula();

                // Mostrar el resultado
                Console.WriteLine($"Formula set successfully. Result: {cell.Value}");

                // Guarda el libro de trabajo
                workbook.Save("SetFormulaDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting formula: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, FormulaParseOptions, object) {#setformula_1}

Establece la fórmula y el valor (resultado calculado) de la fórmula.

```csharp
public void SetFormula(string formula, FormulaParseOptions options, object value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fórmula | String | La fórmula. |
| opciones | FormulaParseOptions | Opciones para analizar la fórmula. |
| valor | Objeto | El valor (resultado calculado) de la fórmula. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringFormulaParseOptionsObjecDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Establezca la fórmula inicial con referencia al complemento
            sheet.Cells[0, 0].Formula = "'externalDS.xlam'!dsfun(B1)";
            Console.WriteLine("Initial formula: " + sheet.Cells[0, 0].Formula);

            // Utilice SetFormula para sobrescribir sin comprobar el complemento
            sheet.Cells[0, 0].SetFormula("=dsfun(B1)", new FormulaParseOptions() { CheckAddIn = false }, null);
            Console.WriteLine("After SetFormula: " + sheet.Cells[0, 0].Formula);

            // Restablecer a la fórmula del complemento
            sheet.Cells[0, 0].Formula = "'externalDS.xlam'!dsfun(B1)";
            Console.WriteLine("Reset to add-in formula: " + sheet.Cells[0, 0].Formula);

            // Crear nuevo libro de trabajo y copiar hoja
            Workbook wb2 = new Workbook();
            wb2.Worksheets[0].Cells[0, 0].Formula = "'externalDS.xlam'!dsfunnew(C1)";
            wb2.Worksheets[0].Copy(sheet);
            Console.WriteLine("After copy: " + wb2.Worksheets[0].Cells[0, 0].Formula);
        }
    }
}
```

### Ver también

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


