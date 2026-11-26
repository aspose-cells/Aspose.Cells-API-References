---
title: "Hyperlink.Address"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Hyperlink. Representa la dirección de un hipervínculo"
type: docs
url: /es/net/aspose.cells/hyperlink/address/
---
## Hyperlink.Address property

Representa la dirección de un hipervínculo.

```csharp
public string Address { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyAddressDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar hipervínculos con direcciones diferentes
            worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.baidu.com/");
            worksheet.Hyperlinks.Add("B1", 1, 1, "http://www.google.com/");
            worksheet.Hyperlinks.Add("C1", 1, 1, "Sheet1!F3");

            // Acceder y mostrar direcciones de hipervínculos
            HyperlinkCollection links = worksheet.Hyperlinks;
            Console.WriteLine("Hyperlink Count: " + links.Count);
            Console.WriteLine("Link 1 Address: " + links[0].Address);
            Console.WriteLine("Link 2 Address: " + links[1].Address);
            Console.WriteLine("Link 3 Address: " + links[2].Address);

            // Guarda el libro de trabajo
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


