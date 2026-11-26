---
title: "StyleFlag.FontStrike"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "StyleFlag propiedad. La configuración de tachado de fuente se aplicará"
type: docs
url: /es/net/aspose.cells/styleflag/fontstrike/
---
## StyleFlag.FontStrike property

Se aplicará la configuración de tachado de fuente.

```csharp
public bool FontStrike { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontStrikeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la celda A1 y establecer algún texto
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Crear un objeto de estilo y establecer FontStrike en true
            Style style = workbook.CreateStyle();
            style.Font.IsStrikeout = true;

            // Crear una bandera de estilo y habilitar la bandera FontStrike
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontStrike = true;

            // Aplicar el estilo a la celda con la bandera de estilo
            cell.SetStyle(style, styleFlag);

            // Mostrar el estado actual de FontStrike
            Console.WriteLine("FontStrike applied: " + cell.GetStyle().Font.IsStrikeout);

            // Crear otra celda para demostrar texto sin tachado
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Normal Text");
            styleFlag.FontStrike = false;

            cell2.SetStyle(style, styleFlag);
            Console.WriteLine("FontStrike applied: " + cell2.GetStyle().Font.IsStrikeout);

            // Guardar el libro de trabajo para ver los efectos
            workbook.Save("PropertyFontStrikeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


