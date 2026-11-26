---
title: "Cell.SetSharedFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Establece una fórmula en un rango de celdas"
type: docs
url: /es/net/aspose.cells/cell/setsharedformula/
---
## SetSharedFormula(string, int, int, bool, bool) {#setsharedformula_3}

Establece una fórmula en un rango de celdas.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, bool isR1C1, 
    bool isLocal)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sharedFormula | String | Fórmula compartida. |
| rowNumber | Int32 | Número de filas para poblar la fórmula. |
| columnNumber | Int32 | Número de columnas para poblar la fórmula. |
| isR1C1 | Booleano | si la fórmula es una fórmula R1C1 |
| isLocal | Booleano | si la fórmula está formateada según la configuración regional |

### Observaciones

NOTA: Esta clase está ahora obsoleta. En su lugar, por favor use Cell.SetSharedFormula(string,int,int,FormulaParseOptions). Esta propiedad será eliminada 12 meses después a partir de diciembre de 2019. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetSharedFormulaWithStringInt32Int32BooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            // Poblar datos de ejemplo en la columna A
            for (int row = 0; row < 5; row++)
            {
                cells[row, 0].Value = row + 1; // A1-A5: 1-5
            }

            // Obtener la celda objetivo B1 para establecer la fórmula compartida
            Cell targetCell = cells[0, 1]; // B1

            try
            {
                // Establecer fórmula compartida para calcular el cuadrado de los valores en la columna A
                // Parámetros: (formula, rowCount=5, columnCount=1, isR1C1=false, isLocal=false)
#pragma warning disable 0618 // Disable obsolete warning for demonstration
                targetCell.SetSharedFormula("=A1^2", 5, 1, false, false);
#pragma warning restore 0618

                // Verificar la propagación de la fórmula
                Console.WriteLine($"B1 formula: {targetCell.Formula}");
                Console.WriteLine($"B5 formula: {cells[4, 1].Formula}");

                // Calcular el libro de trabajo para actualizar los resultados de la fórmula
                workbook.CalculateFormula();

                Console.WriteLine($"A1 value: {cells["A1"].Value}");
                Console.WriteLine($"A5 value: {cells["A5"].Value}");
                Console.WriteLine($"B1 value: {targetCell.Value}");
                Console.WriteLine($"B5 value: {cells[4, 1].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
                return;
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("SetSharedFormulaDemo.xlsx");
            Console.WriteLine("Spreadsheet saved successfully.");
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetSharedFormula(string, int, int) {#setsharedformula}

Establece fórmulas compartidas a un rango de celdas.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sharedFormula | String | Fórmula compartida. |
| rowNumber | Int32 | Número de filas para poblar la fórmula. |
| columnNumber | Int32 | Número de columnas para poblar la fórmula. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetSharedFormulaWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer una fórmula compartida en la columna B desde B1 hasta B20
            cells["B1"].SetSharedFormula("=C1*2", 20, 1);

            // Establecer algunos valores en la columna C para demostrar el cálculo de la fórmula
            for (int i = 0; i < 20; i++)
            {
                cells[i, 2].PutValue(i + 1); // Column C values (C1=1, C2=2...)
            }

            // Calcular fórmulas
            workbook.CalculateFormula();

            // Mostrar resultados para verificación
            for (int i = 0; i < 5; i++) // Display first 5 results
            {
                Console.WriteLine($"B{i+1} value: {cells[i, 1].Value}");
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

## SetSharedFormula(string, int, int, FormulaParseOptions) {#setsharedformula_1}

Establece fórmulas compartidas a un rango de celdas.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sharedFormula | String | Fórmula compartida. |
| rowNumber | Int32 | Número de filas para poblar la fórmula. |
| columnNumber | Int32 | Número de columnas para poblar la fórmula. |
| opciones | FormulaParseOptions | Opciones para analizar la fórmula. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetSharedFormulaWithStringInt32Int32FormulaParseOpDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar datos de ejemplo en la columna A
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Obtener la celda objetivo donde estableceremos la fórmula compartida
            Cell targetCell = worksheet.Cells["B1"];

            try
            {
                // Crear opciones de análisis de fórmula con la configuración predeterminada
                FormulaParseOptions options = new FormulaParseOptions();

                // Establecer fórmula compartida para 3 filas y 2 columnas a partir de B1
                targetCell.SetSharedFormula("=A1*2", 3, 2, options);

                Console.WriteLine("Shared formula set successfully for B1:C3 range");
                Console.WriteLine("B1 formula: " + worksheet.Cells["B1"].Formula);
                Console.WriteLine("C3 formula: " + worksheet.Cells["C3"].Formula);

                workbook.CalculateFormula();
                Console.WriteLine("B3 value: " + worksheet.Cells["B3"].Value);
                Console.WriteLine("B1 value: " + worksheet.Cells["B1"].Value);
                Console.WriteLine("C3 value: " + worksheet.Cells["C3"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("SetSharedFormulaDemo.xlsx");
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

## SetSharedFormula(string, int, int, FormulaParseOptions, object[][]) {#setsharedformula_2}

Establece fórmulas compartidas a un rango de celdas.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options, object[][] values)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sharedFormula | String | Fórmula compartida. |
| rowNumber | Int32 | Número de filas para poblar la fórmula. |
| columnNumber | Int32 | Número de columnas para poblar la fórmula. |
| opciones | FormulaParseOptions | Opciones para analizar la fórmula. |
| values | Object[][] | valores para esas celdas con la fórmula compartida dada |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodSetSharedFormulaWithStringInt32Int32FormulaParseOpDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer valor de muestra en la celda A1
            worksheet.Cells["A1"].PutValue(5);

            // Obtener la celda objetivo B2 donde se establecerá la fórmula compartida
            Cell cell = worksheet.Cells["B2"];

            try
            {
                // Definir parámetros de la fórmula compartida
                string formula = "=A1*2";
                int totalRows = 2;
                int totalColumns = 2;
                FormulaParseOptions parseOptions = new FormulaParseOptions();
                object[][] presetValues = new object[2][]
                {
                    new object[] { 10, 10 },
                    new object[] { 10, 10 }
                };

                // Establecer fórmula compartida para el rango 2x2 que comienza en B2 con valores predefinidos
                cell.SetSharedFormula(formula, totalRows, totalColumns, parseOptions, presetValues);

                Console.WriteLine("Shared formula set successfully. Cells B2:C3 contain values 10");
                workbook.CalculateFormula();
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2", "C3");
                IEnumerator iter = range.GetEnumerator();
                while(iter.MoveNext()) 
                {
                    Cell temp = (Cell)iter.Current;
                    Console.WriteLine(temp.Name + "  " + temp.Value);
                }

            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("SetSharedFormulaDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


