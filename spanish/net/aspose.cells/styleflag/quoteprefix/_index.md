---
title: "StyleFlag.QuotePrefix"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicará la configuración Hide formula"
type: docs
url: /es/net/aspose.cells/styleflag/quoteprefix/
---
## StyleFlag.QuotePrefix property

Se aplicará la configuración de ocultar fórmula.

```csharp
public bool QuotePrefix { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyQuotePrefixDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceda a la celda A1 y establezca un valor que parezca un número pero que debe tratarse como texto
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("123456");

            // Cree un estilo y establezca QuotePrefix a true
            Style style = workbook.CreateStyle();
            style.QuotePrefix = true;

            // Cree una bandera de estilo y habilite la bandera QuotePrefix
            StyleFlag flag = new StyleFlag();
            flag.QuotePrefix = true;

            // Aplique el estilo a la celda usando SetStyle en lugar de ApplyStyle
            cell.SetStyle(style, flag);

            // Muestre el valor actual de QuotePrefix
            Console.WriteLine("Current QuotePrefix value: " + cell.GetStyle().QuotePrefix);

            // Guarde el libro de trabajo para ver el efecto (el valor será tratado como texto en Excel)
            workbook.Save("PropertyQuotePrefixDemo.xlsx");

            // Ahora cambiemos QuotePrefix a false y veamos la diferencia
            style.QuotePrefix = false;
            cell.SetStyle(style, flag);

            Console.WriteLine("Current QuotePrefix value: " + cell.GetStyle().QuotePrefix);
            // Guarde nuevamente con un nombre diferente para comparar
            workbook.Save("PropertyQuotePrefixDemo_WithoutPrefix.xlsx");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


