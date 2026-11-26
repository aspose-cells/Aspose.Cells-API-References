---
title: "TxtSaveOptions.QuoteType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtSaveOptions. Obtiene o establece cómo entrecomillar los valores en el archivo de texto exportado"
type: docs
url: /es/net/aspose.cells/txtsaveoptions/quotetype/
---
## TxtSaveOptions.QuoteType property

Obtiene o establece cómo citar los valores en el archivo de texto exportado.

```csharp
public TxtValueQuoteType QuoteType { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyQuoteTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de muestra con datos de prueba
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Text");
            worksheet.Cells["B1"].PutValue("123");
            worksheet.Cells["A2"].PutValue("Another text");
            worksheet.Cells["B2"].PutValue("=1+2");

            // Guarde con QuoteType.Normal (predeterminado)
            MemoryStream stream1 = new MemoryStream();
            workbook.Save(stream1, new TxtSaveOptions()
            {
                Encoding = Encoding.ASCII
            });
            
            // Guarde con QuoteType.Always
            MemoryStream stream2 = new MemoryStream();
            workbook.Save(stream2, new TxtSaveOptions()
            {
                Encoding = Encoding.ASCII,
                QuoteType = TxtValueQuoteType.Always
            });

            // Mostrar salida de ejemplo
            Console.WriteLine("Normal QuoteType:");
            Console.WriteLine(Encoding.ASCII.GetString(stream1.ToArray()));
            
            Console.WriteLine("\nAlways QuoteType:");
            Console.WriteLine(Encoding.ASCII.GetString(stream2.ToArray()));
        }
    }
}
```

### Ver también

* enum [TxtValueQuoteType](../../txtvaluequotetype/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


