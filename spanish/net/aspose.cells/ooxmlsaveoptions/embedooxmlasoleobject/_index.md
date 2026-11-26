---
title: "OoxmlSaveOptions.EmbedOoxmlAsOleObject"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OoxmlSaveOptions. Indica si se incrustan archivos Ooxml de OleObject como objeto ole"
type: docs
url: /es/net/aspose.cells/ooxmlsaveoptions/embedooxmlasoleobject/
---
## OoxmlSaveOptions.EmbedOoxmlAsOleObject property

Indica si se incrustan archivos Ooxml de OleObject como objeto ole.

```csharp
public bool EmbedOoxmlAsOleObject { get; set; }
```

### Observaciones

Solo para OleObject.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyEmbedOoxmlAsOleObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample OLE Object Embedding");
            
            // Crear opciones de guardado OOXML y establecer EmbedOoxmlAsOleObject
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.EmbedOoxmlAsOleObject = true;
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", saveOptions);
            
            Console.WriteLine("Workbook saved with OOXML embedded as OLE object.");
        }
    }
}
```

### Ver también

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


