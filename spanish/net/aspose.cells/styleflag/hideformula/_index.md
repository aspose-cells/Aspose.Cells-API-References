---
title: "StyleFlag.HideFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicará la configuración Hide formula"
type: docs
url: /es/net/aspose.cells/styleflag/hideformula/
---
## StyleFlag.HideFormula property

Se aplicará la configuración de ocultar fórmula.

```csharp
public bool HideFormula { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyHideFormulaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell a1 = worksheet.Cells["A1"];
            // Agregar una fórmula a la celda A1
            a1.Formula = "=1+2";
            a1.Value = 3; // Display value

            // Crear una bandera de estilo con HideFormula establecida en true
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.HideFormula = true;

            // Crear un estilo y establecer IsFormulaHidden en true
            Style style = workbook.CreateStyle();
            style.IsFormulaHidden = true;

            // Aplicar el estilo a la celda A1 con la bandera de estilo
            a1.SetStyle(style, styleFlag);

            // Proteger la hoja de cálculo para ver el efecto de HideFormula
            worksheet.Protection.AllowEditingObject = true;
            worksheet.Protection.AllowEditingContent = false;
            worksheet.Protection.Password = "password";

            // Guarda el libro de trabajo
            workbook.Save("PropertyHideFormulaDemo.xlsx");

            // Verificar que la fórmula esté oculta
            Console.WriteLine("Formula in A1: " + a1.Formula);
            Console.WriteLine("Is formula hidden? " + a1.GetStyle().IsFormulaHidden);
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


