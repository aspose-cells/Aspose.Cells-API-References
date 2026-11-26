---
title: "Cell.SetArrayFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Establece una fórmula de matriz a un rango de celdas"
type: docs
url: /es/net/aspose.cells/cell/setarrayformula/
---
## SetArrayFormula(string, int, int, bool, bool) {#setarrayformula_3}

Establece una fórmula de matriz a un rango de celdas.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, bool isR1C1, 
    bool isLocal)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arrayFormula | String | Fórmula de matriz. |
| rowNumber | Int32 | Número de filas para poblar el resultado de la fórmula de matriz. |
| columnNumber | Int32 | Número de columnas para poblar el resultado de la fórmula de matriz. |
| isR1C1 | Booleano | si la fórmula es una fórmula R1C1 |
| isLocal | Booleano | si la fórmula está formateada según la configuración regional |

### Observaciones

NOTA: Esta clase está ahora obsoleta. En su lugar, utilice Cell.SetArrayFormula(string,int,int,FormulaParseOptions). Esta propiedad será eliminada 12 meses después desde diciembre de 2019. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetArrayFormulaWithStringInt32Int32BooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;

            try
            {
                // Obtener la celda objetivo donde queremos establecer la fórmula de matriz
                Cell targetCell = worksheet.Cells["B1"];

                // Establecer una fórmula de matriz que multiplique los valores en A1:A3 por 2
                // Parámetros: (formula, rowNumber=3, columnNumber=1, isR1C1=false, isLocal=false)
                targetCell.SetArrayFormula("=A1:A3*2", 3, 1, false, false);

                // Calcular el libro de trabajo para ver los resultados
                workbook.CalculateFormula();

                // Muestra los resultados
                Console.WriteLine($"B1 value: {targetCell.Value}");
                Console.WriteLine($"B2 value: {worksheet.Cells["B2"].Value}");
                Console.WriteLine($"B3 value: {worksheet.Cells["B3"].Value}");

                // Guarda el libro de trabajo
                workbook.Save("SetArrayFormulaDemo.xlsx");
                Console.WriteLine("Array formula set successfully and workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting array formula: {ex.Message}");
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

## SetArrayFormula(string, int, int) {#setarrayformula}

Establece una fórmula de matriz (fórmula de matriz heredada ingresada mediante CTRL+SHIFT+ENTER en MS Excel) a un rango de celdas.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arrayFormula | String | Fórmula de matriz. |
| rowNumber | Int32 | Número de filas para poblar el resultado de la fórmula de matriz. |
| columnNumber | Int32 | Número de columnas para poblar el resultado de la fórmula de matriz. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetArrayFormulaWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            Cell cell = cells["A1"];
            cell.SetArrayFormula("=FREQUENCY({\"79\",\"85\",\"78\",\"85\",\"50\",\"81\",\"95\",\"88\",\"97\"},{70,79,89})", 4, 1);

            workbook.CalculateFormula();

            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1} value: {cells[i, 0].IntValue}");
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

## SetArrayFormula(string, int, int, FormulaParseOptions) {#setarrayformula_1}

Establece una fórmula de matriz a un rango de celdas.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arrayFormula | String | Fórmula de matriz. |
| rowNumber | Int32 | Número de filas para poblar el resultado de la fórmula de matriz. |
| columnNumber | Int32 | Número de columnas para poblar el resultado de la fórmula de matriz. |
| opciones | FormulaParseOptions | Opciones para analizar la fórmula. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetArrayFormulaWithStringInt32Int32FormulaParseOpDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Colocar datos de ejemplo en las celdas C1:E1
            cells["C1"].PutValue(10);
            cells["D1"].PutValue(20);
            cells["E1"].PutValue(30);

            // Establecer fórmula de matriz en la celda A1 que se expandirá a 2 filas y 3 columnas
            cells["A1"].SetArrayFormula("=TRANSPOSE(C1:E1)", 2, 1, new FormulaParseOptions());

            // Calcular fórmulas
            workbook.CalculateFormula();

            // Genere la salida de los resultados
            Console.WriteLine("Array formula results:");
            for (int row = 0; row < 2; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Cell cell = cells[row, col];
                    Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                }
            }
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

## SetArrayFormula(string, int, int, FormulaParseOptions, object[][]) {#setarrayformula_2}

Establece una fórmula de matriz a un rango de celdas.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options, object[][] values)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arrayFormula | String | Fórmula de matriz. |
| rowNumber | Int32 | Número de filas para poblar el resultado de la fórmula de matriz. |
| columnNumber | Int32 | Número de columnas para poblar el resultado de la fórmula de matriz. |
| opciones | FormulaParseOptions | Opciones para analizar la fórmula. |
| values | Object[][] | valores para esas celdas con la fórmula de matriz dada |

### Ver también

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


