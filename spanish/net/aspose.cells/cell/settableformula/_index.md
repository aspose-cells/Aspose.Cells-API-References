---
title: "Cell.SetTableFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Crear tabla de datos de dos variables para el rango dado que comienza desde esta celda"
type: docs
url: /es/net/aspose.cells/cell/settableformula/
---
## SetTableFormula(int, int, string, string, object[][]) {#settableformula_3}

Crear tabla de datos de dos variables para el rango dado comenzando desde esta celda.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string rowInputCell, 
    string columnInputCell, object[][] values)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowNumber | Int32 | Número de filas para poblar la fórmula. |
| columnNumber | Int32 | Número de columnas para poblar la fórmula. |
| rowInputCell | String | la celda de entrada de fila |
| columnInputCell | String | la celda de entrada de columna |
| values | Object[][] | valores para las celdas en el rango de la fórmula de tabla |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32StringStringObjectArrayDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(2);
            cells[1, 3].PutValue(3);
            cells[2, 1].PutValue(2);
            cells[3, 1].PutValue(3);
            cells[4, 1].PutValue(4);

            // Celda objetivo donde se establecerá la fórmula de tabla
            Cell targetCell = worksheet.Cells["C3"];

            // Preparar parámetros para SetTableFormula
            int rowNumber = 3;
            int columnNumber = 2;
            string rowInputCell = "A1";
            string columnInputCell = "A2";
            object[][] values = new object[][]
            {
                new object[] { 1, 2 },    // Row 1 data
                new object[] { 3, 4 },    // Row 2 data
                new object[] { 5, 6 }     // Row 3 data
            };

            try
            {
                // Establecer la fórmula de tabla en la celda objetivo
                targetCell.SetTableFormula(rowNumber, columnNumber, rowInputCell, columnInputCell, values);

                // Calcular fórmulas del libro de trabajo para actualizar los resultados
                workbook.CalculateFormula();

                Console.WriteLine("Table formula set successfully. Check D1:" + targetCell.StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("SetTableFormulaDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, string, bool, object[][]) {#settableformula_2}

Crear tabla de datos de una variable para el rango dado comenzando desde esta celda.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string inputCell, bool isRowInput, 
    object[][] values)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowNumber | Int32 | Número de filas para poblar la fórmula. |
| columnNumber | Int32 | Número de columnas para poblar la fórmula. |
| inputCell | String | la celda de entrada |
| isRowInput | Booleano | Indica si la celda de entrada es una celda de entrada de fila (true) o una celda de entrada de columna (false). |
| values | Object[][] | valores para las celdas en el rango de la fórmula de tabla |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32StringBooleanObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = worksheet.Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(100000);
            cells[1, 3].PutValue(0.05);
            cells[1, 4].PutValue(2);
            cells[2, 1].PutValue(360);
            cells[3, 1].PutValue(30);
            cells[4, 1].PutValue(40);
            
            try
            {
                // Preparar parámetros para SetTableFormula
                int rowCount = 3;
                int colCount = 3;
                object[][] inputValues = new object[][] 
                {
                    new object[] { 0.05, 0.06, 0.07 },
                    new object[] { 1000, 2000, 3000 },
                    new object[] { 100, 200, 300 }
                };

                // Obtener la celda objetivo para la tabla de datos (C3)
                Cell tableCell = worksheet.Cells["C3"];
                // Llamar a SetTableFormula con variaciones de la tasa de interés
                tableCell.SetTableFormula(
                    rowNumber: rowCount,
                    columnNumber: colCount,
                    inputCell: "A1",
                    isRowInput: true,
                    values: inputValues
                );

                // Calcular fórmulas para actualizar los resultados de la tabla
                workbook.CalculateFormula();

                Console.WriteLine("Data table created successfully with varying interest rates");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating data table: {ex.Message}");
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("SetTableFormulaDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, int, int, int, int, object[][]) {#settableformula_1}

Crear tabla de datos de dos variables para el rango dado comenzando desde esta celda.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, 
    int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, 
    object[][] values)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowNumber | Int32 | Número de filas para poblar la fórmula. |
| columnNumber | Int32 | Número de columnas para poblar la fórmula. |
| rowIndexOfRowInputCell | Int32 | índice de fila de la celda de entrada de fila |
| columnIndexOfRowInputCell | Int32 | índice de columna de la celda de entrada de fila |
| rowIndexOfColumnInputCell | Int32 | índice de fila de la celda de entrada de columna |
| columnIndexOfColumnInputCell | Int32 | índice de columna de la celda de entrada de columna |
| values | Object[][] | valores para las celdas en el rango de la fórmula de tabla |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(2);
            cells[1, 3].PutValue(3);
            cells[1, 4].PutValue(4);
            cells[2, 1].PutValue(2);
            cells[3, 1].PutValue(3);
            cells[4, 1].PutValue(4);
            
            Cell formulaCell = cells[2, 2];

            // Preparar valores de entrada para la tabla de datos (tasas de interés y montos de préstamo)
            object[][] tableValues = new object[3][];
            tableValues[0] = new object[] { 0.05, 0.06, 0.07 };
            tableValues[1] = new object[] { 1000, 2000, 3000 };
            tableValues[2] = new object[] { 100, 200, 300 };

            try
            {
                // Establecer la fórmula de tabla con dimensiones de tabla de datos 3x3 y desplazamientos de la celda de entrada
                formulaCell.SetTableFormula(
                    rowNumber: 3,
                    columnNumber: 3,
                    rowIndexOfRowInputCell: 0,  
                    columnIndexOfRowInputCell: 0,   
                    rowIndexOfColumnInputCell: 1,   
                    columnIndexOfColumnInputCell: 0, 
                    values: tableValues
                );

                workbook.CalculateFormula();
                Console.WriteLine("Data table formula set successfully. Check B2:D4 in output.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            workbook.Save("CellTableFormulaDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, int, int, bool, object[][]) {#settableformula}

Crear tabla de datos de una variable para el rango dado comenzando desde esta celda.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, 
    int columnIndexOfInputCell, bool isRowInput, object[][] values)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowNumber | Int32 | Número de filas para poblar la fórmula. |
| columnNumber | Int32 | Número de columnas para poblar la fórmula. |
| rowIndexOfInputCell | Int32 | índice de fila de la celda de entrada |
| columnIndexOfInputCell | Int32 | índice de columna de la celda de entrada |
| isRowInput | Booleano | Indica si la celda de entrada es una celda de entrada de fila (true) o una celda de entrada de columna (false). |
| values | Object[][] | valores para las celdas en el rango de la fórmula de tabla |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32Int32Int32BooleanObjDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(20);
            cells[1, 3].PutValue(30);            
            cells[2, 1].PutValue(20);
            cells[3, 1].PutValue(30);
            cells[4, 1].PutValue(40);

            // Crear matriz de datos de muestra para los parámetros de la fórmula de tabla
            object[][] inputValues = new object[][]
            {
                new object[] { 10, 20 },
                new object[] { 30, 40 },
                new object[] { 50, 60 }
            };

            // Obtener la celda objetivo para aplicar la fórmula de tabla
            Cell formulaCell = worksheet.Cells[2, 2];

            try
            {
                // Establecer fórmula de tabla con: 
                // 3 filas, 2 columnas, celda de entrada en A1 (0,0), 
                // tipo de entrada de fila y valores de muestra
                formulaCell.SetTableFormula(
                    rowNumber: 3,
                    columnNumber: 2,
                    rowIndexOfInputCell: 0,
                    columnIndexOfInputCell: 0,
                    isRowInput: true,
                    values: inputValues
                );

                workbook.CalculateFormula();
                Console.WriteLine("Table formula applied successfully. " + 
                    "Saved workbook with 3x2 table formula at C3.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("TableFormulaDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


