---
title: "FormulaParseOptions.CheckAddIn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormulaParseOptions. Indica si se verifican los complementos en los enlaces externos existentes del libro actual para funciones definidas por el usuario sin enlace externo. El valor predeterminado es true. Si la función definida por el usuario coincide con un complemento en los enlaces externos existentes, se tomará como ese complemento."
type: docs
url: /es/net/aspose.cells/formulaparseoptions/checkaddin/
---
## FormulaParseOptions.CheckAddIn property

Indica si se deben comprobar los complementos en los enlaces externos existentes del libro actual para funciones definidas por el usuario sin enlace externo. El valor predeterminado es true (si la función definida por el usuario coincide con un complemento en los enlaces externos existentes, se toma como el complemento).

```csharp
public bool CheckAddIn { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyCheckAddInDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Registrar función de complemento
            wb.Worksheets.RegisterAddInFunction("Test.xlam", "TEST_UDF", false);

            // Sin CheckAddIn=false - la fórmula se convertirá al formato de complemento
            cells["A1"].SetFormula("=TEST_UDF()", new FormulaParseOptions());
            Console.WriteLine("A1 Formula (CheckAddIn=true): " + cells["A1"].Formula);

            // Con CheckAddIn=false - la fórmula permanece sin cambios
            cells["A2"].SetFormula("=TEST_UDF()", new FormulaParseOptions() { CheckAddIn = false });
            Console.WriteLine("A2 Formula (CheckAddIn=false): " + cells["A2"].Formula);
        }
    }
}
```

### Ver también

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


