---
title: "TxtSaveOptions.AlwaysQuoted"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtSaveOptions. Indica si siempre se agrega  para cada campo. Si es true, entonces todos los valores estarán entre comillas. Si es false, los valores solo estarán entre comillas cuando sea necesario, por ejemplo cuando los valores contengan caracteres especiales como   n o el carácter separador. El valor predeterminado es false."
type: docs
url: /es/net/aspose.cells/txtsaveoptions/alwaysquoted/
---
## TxtSaveOptions.AlwaysQuoted property

Indica si siempre se agrega '\"' para cada campo. Si es true, entonces todos los valores estarán entre comillas; si es false, los valores solo estarán entre comillas cuando sea necesario (por ejemplo, cuando los valores contengan caracteres especiales como '\"', '\\n' o el carácter separador). El valor predeterminado es false.

```csharp
[Obsolete("Use QuoteType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AlwaysQuoted { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad QuoteType. Esta propiedad será eliminada 12 meses después desde agosto de 2012. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyAlwaysQuotedDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200.50);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(899.99);

            // Cree TxtSaveOptions con AlwaysQuoted establecido en true
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Separator = ',',
                AlwaysQuoted = true,
                QuoteType = TxtValueQuoteType.Always
            };

            // Guarde con comillas alrededor de todos los valores
            workbook.Save("AlwaysQuoted_True.txt", saveOptions);

            // Cambie a false y guarde nuevamente
            saveOptions.AlwaysQuoted = false;
            workbook.Save("AlwaysQuoted_False.txt", saveOptions);

            Console.WriteLine("Files saved with different AlwaysQuoted settings.");
        }
    }
}
```

### Ver también

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


