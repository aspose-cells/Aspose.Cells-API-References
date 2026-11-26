---
title: "FormatCondition.GetFormula2"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FormatCondition. Obtiene el valor o expresión asociado con esta condición de formato"
type: docs
url: /es/net/aspose.cells/formatcondition/getformula2/
---
## GetFormula2(bool, bool) {#getformula2}

Obtiene el valor o expresión asociado a esta condición de formato.

```csharp
public string GetFormula2(bool isR1C1, bool isLocal)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | Booleano | Si la fórmula necesita formatearse como R1C1. |
| isLocal | Booleano | Si la fórmula necesita formatearse según la configuración regional. |

### Valor de retorno

El valor o expresión asociado con esta condición de formato.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodGetFormula2WithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Agregar una condición de formato
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 2;
            area.StartColumn = 0;
            area.EndColumn = 0;
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");
            FormatCondition fc = fcs[conditionIndex];
            
            // Establecer Formula2
            fc.Formula2 = "30";

            try
            {
                // Llamar a GetFormula2 con parámetros (Boolean, Boolean)
                string formula2 = fc.GetFormula2(false, false);
                
                // Mostrar el resultado
                Console.WriteLine("Formula2: " + formula2);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("FormatConditionMethodGetFormula2WithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula2(bool, bool, int, int) {#getformula2_1}

Obtiene el valor o expresión del formato condicional de la celda.

```csharp
public string GetFormula2(bool isR1C1, bool isLocal, int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | Booleano | Si la fórmula necesita formatearse como R1C1. |
| isLocal | Booleano | Si la fórmula necesita formatearse según la configuración regional. |
| fila | Int32 | El índice de fila. |
| columna | Int32 | El índice de columna. |

### Valor de retorno

El valor o expresión asociado con el formato condicional de la celda.

### Observaciones

La celda dada debe estar contenida en este formato condicional, de lo contrario se devolverá null.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodGetFormula2WithBooleanBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Agregar un formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A1", "=A3");
            FormatCondition fc = fcs[conditionIndex];

            try
            {
                // Llamar a GetFormula2 con parámetros específicos (isR1C1, isLocal, row, column)
                string formula = fc.GetFormula2(false, false, 0, 0);
                
                Console.WriteLine("Formula2 retrieved successfully: " + formula);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean, Int32, Int32)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("FormatConditionMethodGetFormula2WithBooleanBooleanInt32Int32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula2(int, int) {#getformula2_2}

Obtiene la fórmula del formato condicional de la celda.

```csharp
public string GetFormula2(int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | El índice de fila. |
| columna | Int32 | El índice de columna. |

### Valor de retorno

La fórmula.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodGetFormula2WithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(15);
            worksheet.Cells["A3"].PutValue(25);
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Agregar formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 1;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "A1", "B3");

            // Obtener la primera condición de formato
            FormatCondition fc = fcc[0];

            try
            {
                // Llamar a GetFormula2 con parámetros específicos de fila y columna
                string formula = fc.GetFormula2(1, 0); // Row 1, Column 0 (A2)
                
                Console.WriteLine("Formula2 for cell (1,0): " + formula);
                Console.WriteLine("Method executed successfully with parameters (Int32, Int32)");

                // Aplicar estilo para visualizar el formato condicional
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Red;
                fc.Style = style;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("FormatConditionMethodGetFormula2WithInt32Int32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


