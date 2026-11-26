---
title: "Workbook.RefreshDynamicArrayFormulas"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Workbook. Actualiza los derrames de fórmulas de matrices dinámicas a un nuevo rango de celdas vecinas según los datos actuales. Otras fórmulas en el libro no se calcularán de forma recursiva, incluso si fueron utilizadas por fórmulas de matrices dinámicas."
type: docs
url: /es/net/aspose.cells/workbook/refreshdynamicarrayformulas/
---
## RefreshDynamicArrayFormulas(bool) {#refreshdynamicarrayformulas}

Actualiza las fórmulas de matrices dinámicas (desbordan en un nuevo rango de celdas vecinas según los datos actuales). Otras fórmulas en el libro de trabajo no se calcularán de forma recursiva aunque hayan sido utilizadas por fórmulas de matrices dinámicas.

```csharp
public void RefreshDynamicArrayFormulas(bool calculate)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| calcular | Booleano | Indica si calcula y actualiza los valores de celda para esas fórmulas de matrices dinámicas |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRefreshDynamicArrayFormulasWithBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet1 = wb.Worksheets[0];
            Worksheet sheet2 = wb.Worksheets.Add("Sheet2");

            // Configura los datos iniciales y las fórmulas de matrices dinámicas
            sheet1.Cells["A1"].PutValue("B1:B3");
            sheet1.Cells["A2"].SetDynamicArrayFormula("=INDIRECT(A1)", new FormulaParseOptions(), true);
            sheet2.Cells["B1"].SetDynamicArrayFormula("=TRANSPOSE(Sheet1!A2#)", new FormulaParseOptions(), true);

            Console.WriteLine("Before refresh:");
            PrintSpillStatus(sheet1, sheet2);

            // Cambia el rango y actualiza las fórmulas
            sheet1.Cells["A1"].PutValue("B1:B5");
            wb.RefreshDynamicArrayFormulas(true);

            Console.WriteLine("\nAfter refresh:");
            PrintSpillStatus(sheet1, sheet2);
        }

        private static void PrintSpillStatus(Worksheet sheet1, Worksheet sheet2)
        {
            Console.WriteLine("Sheet1 spill range:");
            for (int i = 1; i <= 6; i++)
            {
                Cell cell = sheet1.Cells.CheckCell(i, 0);
                Console.WriteLine($"Row {i}: {(cell != null && cell.IsFormula ? "Formula" : "Empty")}");
            }

            Console.WriteLine("\nSheet2 spill range:");
            for (int i = 1; i <= 6; i++)
            {
                Cell cell = sheet2.Cells.CheckCell(0, i);
                Console.WriteLine($"Column {i}: {(cell != null && cell.IsFormula ? "Formula" : "Empty")}");
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

## RefreshDynamicArrayFormulas(bool, CalculationOptions) {#refreshdynamicarrayformulas_1}

Actualiza las fórmulas de matrices dinámicas (desbordan en un nuevo rango de celdas vecinas según los datos actuales).

```csharp
public void RefreshDynamicArrayFormulas(bool calculate, CalculationOptions copts)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| calcular | Booleano | Indica si calcula y actualiza los valores de celda para esas fórmulas de matrices dinámicas |
| copts | CalculationOptions | Las opciones para calcular fórmulas |

### Observaciones

Por consideraciones de rendimiento, no actualizamos automáticamente todas las fórmulas de matrices dinámicas cuando la propia fórmula o los datos a los que hace referencia cambian. Por lo tanto, el usuario debe llamar a este método manualmente después de aquellas operaciones que puedan influir en las fórmulas de matrices dinámicas, como importar/establecer valores de celda, insertar/eliminar filas/columnas/rangos, etc. Para la mayoría de las fórmulas con funciones, calcular el rango de derrame también requiere calcular la fórmula, por lo que, en general, se prefiere el valor verdadero para la bandera "calculate". Si la fórmula es simple, como una referencia de rango o una matriz (por ejemplo "=C1:E5", "={1,2;3,4}", ...), una función simple sobre un rango o matriz (por ejemplo "=ABS(C1:E5)", "=1+{1,2;3,4}", ...), y todas las fórmulas se calcularán más tarde (por ejemplo mediante [`CalculateFormula`](../calculateformula/)), entonces usar el valor falso para la bandera "calculate" puede evitar el cálculo duplicado en beneficio del rendimiento.

### Ejemplos

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRefreshDynamicArrayFormulasWithBooleanCalculationOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar fórmula de matriz dinámica de ejemplo
            worksheet.Cells["A1"].Formula = "=SEQUENCE(5)";
            
            // Crear opciones de cálculo
            CalculationOptions opts = new CalculationOptions();
            opts.CalcStackSize = 100;
            
            // Actualizar fórmulas de matrices dinámicas con opciones de cálculo
            workbook.RefreshDynamicArrayFormulas(true, opts);
            
            // Calcular fórmulas del workbook
            workbook.CalculateFormula(opts);
            
            // Mostrar resultado de A1:A5
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + (i + 1)].Value);
            }
        }
    }
}
```

### Ver también

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


