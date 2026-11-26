---
title: "FormulaParseOptions.Parse"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormulaParseOptions. Indica si se analiza la fórmula dada. El valor predeterminado es true. Si es false, la cadena de fórmula proporcionada se mantendrá tal cual para la celda hasta que el usuario llame a otros métodos para analizarla o los datos de fórmula analizada sean requeridos por otras operaciones, como el cálculo de fórmulas."
type: docs
url: /es/net/aspose.cells/formulaparseoptions/parse/
---
## FormulaParseOptions.Parse property

Indica si se debe analizar la fórmula proporcionada. El valor predeterminado es true. Si es false, la cadena de fórmula proporcionada se mantendrá tal cual en la celda hasta que el usuario llame a otros métodos para analizarla o se requieran los datos de la fórmula analizada por otras operaciones, como calcular fórmulas.

```csharp
public bool Parse { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyParseDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Establecer fórmulas con Parse=false (las fórmulas no se analizarán inmediatamente)
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["B1"].SetFormula("=A1+A2", new FormulaParseOptions() { Parse = false });
            cells["B2"].SetFormula("=SUM(A1:A2)", new FormulaParseOptions() { Parse = false });

            // Calcular fórmulas (el análisis se realizará ahora)
            wb.CalculateFormula();

            Console.WriteLine("B1 value: " + cells["B1"].Value);
            Console.WriteLine("B2 value: " + cells["B2"].Value);
        }
    }
}
```

### Ver también

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


