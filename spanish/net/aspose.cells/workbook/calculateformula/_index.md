---
title: "Workbook.CalculateFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Calcula el resultado de las fórmulas"
type: docs
url: /es/net/aspose.cells/workbook/calculateformula/
---
## CalculateFormula() {#calculateformula}

Calcula el resultado de las fórmulas.

```csharp
public void CalculateFormula()
```

### Observaciones

Para todas las fórmulas compatibles, consulte la lista en https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Establecer valores y fórmulas
            cells["A1"].PutValue(5);
            cells["B1"].Formula = "=A1*2";
            cells["C1"].Formula = "=B1+10";
            
            // Calcular fórmulas
            workbook.CalculateFormula();
            
            // Mostrar resultados
            Console.WriteLine("A1 value: " + cells["A1"].IntValue);
            Console.WriteLine("B1 formula result: " + cells["B1"].IntValue);
            Console.WriteLine("C1 formula result: " + cells["C1"].IntValue);
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(bool) {#calculateformula_2}

Calcula el resultado de las fórmulas.

```csharp
public void CalculateFormula(bool ignoreError)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ignoreError | Booleano | Indica si se oculta el error al calcular fórmulas. El error puede ser una función no compatible, enlaces externos, etc. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaWithBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            
            // Acceder a la primera hoja de cálculo y sus celdas
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Colocar valores en la primera fila (A1:E1)
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(i + 1); // Values 1-5
            }

            // Colocar valores en la segunda fila (A2:E2)
            for (int i = 0; i < 5; i++)
            {
                cells[1, i].PutValue((i + 1) * 10); // Values 10,20,30,40,50
            }

            // Establecer una fórmula HLOOKUP compartida en la cuarta fila (A4:E4)
            cells[3, 0].SetSharedFormula("=HLOOKUP(A1,$A$1:$E$2,2,FALSE)", 1, 5);

            // Calcular fórmulas sin cálculo recursivo
            wb.CalculateFormula(false);

            // Muestra los resultados
            Console.WriteLine("Formula calculation results:");
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine($"Cell {((char)('A' + i))}4 value: {cells[3, i].StringValue}");
            }
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(CalculationOptions) {#calculateformula_1}

Calculando fórmulas en este libro de trabajo.

```csharp
public void CalculateFormula(CalculationOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opciones | CalculationOptions | Opciones de cálculo |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaWithCalculationOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Crear una tabla y establecer nombres de columna
            sheet.Cells["A1"].PutValue("A");
            sheet.Cells["B1"].PutValue("B");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue(2);
            
            // Establecer fórmulas y calcular
            Cells cells = sheet.Cells;
            cells["C1"].PutValue("InvalidColumn");
            cells["D1"].Formula = "=INDIRECT(\"A\"&ROW())";
            cells["E1"].Formula = "=IFERROR(INDIRECT(\"B\"&ROW()),\"OK\")";
            
            // Calcular fórmulas con opciones
            wb.CalculateFormula(new CalculationOptions());
            
            // Mostrar resultados
            Console.WriteLine("D1 result: " + cells["D1"].StringValue);
            Console.WriteLine("E1 result: " + cells["E1"].StringValue);
        }
    }
}
```

### Ver también

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


