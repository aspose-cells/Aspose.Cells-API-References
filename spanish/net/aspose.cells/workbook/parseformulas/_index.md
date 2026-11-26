---
title: "Workbook.ParseFormulas"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Analiza todas las fórmulas que no se habían analizado cuando se cargaron desde un archivo de plantilla o se establecieron en una celda"
type: docs
url: /es/net/aspose.cells/workbook/parseformulas/
---
## Workbook.ParseFormulas method

Analiza todas las fórmulas que no se han analizado cuando se cargaron desde el archivo de plantilla o se establecieron en una celda.

```csharp
public void ParseFormulas(bool ignoreError)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ignoreError | Booleano | Indica si se ignora el error para una fórmula inválida. Para una fórmula inválida, si se ignora el error, entonces esa fórmula será omitida y el proceso continuará analizando otras fórmulas; de lo contrario se lanzará una excepción. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodParseFormulasWithBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer fórmulas sin analizar (Parse = false)
            for (int i = 1; i < 10; i++)
            {
                cells[i, 0].SetFormula($"=SUM(A{i}:B{i})", new FormulaParseOptions() { Parse = false }, null);
            }

            Console.WriteLine("Formulas set without parsing. Now parsing them all at once...");

            // Analizar todas las fórmulas de una vez
            wb.ParseFormulas(false);

            // Verificar las fórmulas
            for (int i = 1; i < 10; i++)
            {
                Console.WriteLine($"Cell A{i} formula: {cells[i, 0].Formula}");
            }
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


