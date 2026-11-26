---
title: "TxtSaveOptions.ExportQuotePrefix"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtSaveOptions. Indica si el signo de comilla simple debe exportarse como parte del valor de una celda cuando QuotePrefix es true para ella. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/txtsaveoptions/exportquoteprefix/
---
## TxtSaveOptions.ExportQuotePrefix property

Indica si el signo de comilla simple debe exportarse como parte del valor de una celda cuando [`QuotePrefix`](../../style/quoteprefix/) es true para ella. El valor predeterminado es false.

```csharp
public bool ExportQuotePrefix { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyExportQuotePrefixDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Agregar datos de ejemplo con caracteres especiales
            cells[0, 0].PutValue("a\\bcdef\"g");
            cells[0, 1].PutValue("f\"g");
            cells[0, 2].PutValue("a\\bcdg");
            cells[0, 3].PutValue("abcdefg");
            cells[0, 4].PutValue("efg");
            cells[0, 5].PutValue("'abc");

            // Crear opciones de guardado TXT
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                Separator = ',',
                ExportQuotePrefix = true // Demonstrate ExportQuotePrefix property
            };

            // Guardar con ExportQuotePrefix = true
            workbook.Save("output_with_exportquoteprefix.csv", saveOptions);

            // Cambiar el separador y guardar de nuevo
            saveOptions.Separator = '\\';
            workbook.Save("output_with_backslash_separator.csv", saveOptions);

            Console.WriteLine("Files saved successfully with ExportQuotePrefix property.");
        }
    }
}
```

### Ver también

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


