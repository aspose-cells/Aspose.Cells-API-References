---
title: "TxtSaveOptions.Encoding"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtSaveOptions. Obtiene y establece la codificación predeterminada"
type: docs
url: /es/net/aspose.cells/txtsaveoptions/encoding/
---
## TxtSaveOptions.Encoding property

Obtiene y establece la codificación predeterminada.

```csharp
public Encoding Encoding { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyEncodingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            
            // Cree opciones de guardado TXT con codificación ASCII
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                Separator = '\t'
            };
            
            // Guarde el libro de trabajo con la codificación especificada
            workbook.Save("output.txt", saveOptions);
            
            Console.WriteLine("File saved with ASCII encoding");
        }
    }
}
```

### Ver también

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


