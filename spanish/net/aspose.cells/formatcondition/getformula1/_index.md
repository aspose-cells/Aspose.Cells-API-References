---
title: "FormatCondition.GetFormula1"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FormatCondition. Obtiene el valor o expresión asociado con esta condición de formato"
type: docs
url: /es/net/aspose.cells/formatcondition/getformula1/
---
## GetFormula1(bool, bool) {#getformula1}

Obtiene el valor o expresión asociado a esta condición de formato.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal)
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

    public class FormatConditionMethodGetFormula1WithBooleanBooleanDemo
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
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 2;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // Obtener la primera condición de formato
            FormatCondition fc = fcc[0];

            try
            {
                // Llamar a GetFormula1 con parámetros (Boolean, Boolean)
                string formula = fc.GetFormula1(false, false);
                
                Console.WriteLine("Formula1: " + formula);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean)");
                
                // Muestra el efecto mostrando el rango de formato condicional
                Console.WriteLine($"Conditional format applied to range: A1:A3");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula1 method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("FormatConditionMethodGetFormula1WithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula1(bool, bool, int, int) {#getformula1_1}

Obtiene el valor o expresión del formato condicional de la celda.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal, int row, int column)
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
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionMethodGetFormula1WithBooleanBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una condición de formato
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[formatIndex];
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 1, 0));
            int conditionIndex = fcc.AddCondition(FormatConditionType.Expression, OperatorType.None, "=IF(MOD(A1,2)=0,TRUE,FALSE)", null);

            // Obtén la fórmula con diferentes parámetros
            FormatCondition condition = fcc[conditionIndex];
            string formula1 = condition.GetFormula1(false, false, 0, 0);
            string formula2 = condition.GetFormula1(false, false, 1, 0);

            Console.WriteLine("Formula for row 0: " + formula1);
            Console.WriteLine("Formula for row 1: " + formula2);
        }
    }
}
```

### Ver también

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula1(int, int) {#getformula1_2}

Obtiene la fórmula del formato condicional de la celda.

```csharp
public string GetFormula1(int row, int column)
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

    public class FormatConditionMethodGetFormula1WithInt32Int32Demo
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

            // Agregar formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 0;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // Obtener la primera condición de formato
            FormatCondition fc = fcc[0];

            try
            {
                // Llama a GetFormula1 con parámetros específicos de fila y columna
                string formula = fc.GetFormula1(0, 0);
                
                Console.WriteLine("Formula1 for cell (0,0): " + formula);
                Console.WriteLine("Method executed successfully with parameters (Int32, Int32)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula1 method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("FormatConditionMethodGetFormula1WithInt32Int32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


