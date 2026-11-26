---
title: "HtmlSaveOptions.ExportFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se exportan fórmulas al guardar el archivo en html. El valor predeterminado es true. Si deseas importar el html de salida a Excel, por favor mantén el valor predeterminado"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exportformula/
---
## HtmlSaveOptions.ExportFormula property

Indica si se exportan fórmulas al guardar el archivo en html. El valor predeterminado es true. Si desea importar el html generado a Excel, mantenga el valor predeterminado.

```csharp
public bool ExportFormula { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportFormulaDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra y fórmula
            worksheet.Cells["A1"].PutValue("Value 1");
            worksheet.Cells["B1"].PutValue("Value 2");
            worksheet.Cells["C1"].Formula = "=A1+B1";
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["C2"].Formula = "=A2+B2";

            // Guardar con ExportFormula = true
            HtmlSaveOptions options1 = new HtmlSaveOptions();
            options1.ExportFormula = true;
            workbook.Save("output_with_formulas.html", options1);

            // Guardar con ExportFormula = false
            HtmlSaveOptions options2 = new HtmlSaveOptions();
            options2.ExportFormula = false;
            workbook.Save("output_without_formulas.html", options2);

            // Verifique los resultados
            string htmlWithFormulas = File.ReadAllText("output_with_formulas.html");
            string htmlWithoutFormulas = File.ReadAllText("output_without_formulas.html");

            Console.WriteLine("HTML with formulas contains formula: " + 
                htmlWithFormulas.Contains("=A2+B2"));
            Console.WriteLine("HTML without formulas contains formula: " + 
                htmlWithoutFormulas.Contains("=A2+B2"));
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


