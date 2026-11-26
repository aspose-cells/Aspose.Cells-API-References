---
title: "Font.IsSubscript"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Font. Obtiene o establece un valor que indica si la fuente está en subíndice"
type: docs
url: /es/net/aspose.cells/font/issubscript/
---
## Font.IsSubscript property

Obtiene o establece un valor que indica si la fuente está en subíndice.

```csharp
public bool IsSubscript { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsSubscriptDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un estilo con texto en subíndice
            Style subscriptStyle = workbook.CreateStyle();
            subscriptStyle.Font.IsSubscript = true;

            // Crear un estilo con texto en superíndice para comparación
            Style superscriptStyle = workbook.CreateStyle();
            superscriptStyle.Font.IsSuperscript = true;

            // Aplicar estilos a las celdas
            worksheet.Cells["A1"].PutValue("Subscript Text");
            worksheet.Cells["A1"].SetStyle(subscriptStyle);

            worksheet.Cells["A2"].PutValue("Superscript Text");
            worksheet.Cells["A2"].SetStyle(superscriptStyle);

            // Verificar y mostrar los estilos
            Console.WriteLine("A1 IsSubscript: " + worksheet.Cells["A1"].GetStyle().Font.IsSubscript);
            Console.WriteLine("A1 IsSuperscript: " + worksheet.Cells["A1"].GetStyle().Font.IsSuperscript);
            Console.WriteLine("A2 IsSubscript: " + worksheet.Cells["A2"].GetStyle().Font.IsSubscript);
            Console.WriteLine("A2 IsSuperscript: " + worksheet.Cells["A2"].GetStyle().Font.IsSuperscript);

            // Guarda el libro de trabajo
            workbook.Save("FontPropertyIsSubscriptDemo.ods");
        }
    }
}
```

### Ver también

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


