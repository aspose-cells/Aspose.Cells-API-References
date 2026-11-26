---
title: "Font.IsSuperscript"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Font. Obtiene o establece un valor que indica si la fuente está en superíndice"
type: docs
url: /es/net/aspose.cells/font/issuperscript/
---
## Font.IsSuperscript property

Obtiene o establece un valor que indica si la fuente está en superíndice.

```csharp
public bool IsSuperscript { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsSuperscriptDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar texto a la celda A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Normal Text Superscript Text");
            
            // Formatear parte del texto como superíndice
            FontSetting setting = cell.Characters(12, 11);
            setting.Font.IsSuperscript = true;
            
            // Guarda el libro de trabajo
            workbook.Save("FontIsSuperscriptDemo.xlsx");
            
            // Verifique la configuración de superíndice
            Console.WriteLine("IsSuperscript property: " + setting.Font.IsSuperscript);
        }
    }
}
```

### Ver también

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


