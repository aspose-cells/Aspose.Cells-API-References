---
title: "VbaModule.BinaryCodes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VbaModule. Obtiene y establece los códigos binarios del módulo"
type: docs
url: /es/net/aspose.cells.vba/vbamodule/binarycodes/
---
## VbaModule.BinaryCodes property

Obtiene y establece los códigos binarios del módulo.

```csharp
public byte[] BinaryCodes { get; }
```

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyBinaryCodesDemo
    {
        public static void Run()
        {
            // Cargar el libro de trabajo con proyecto VBA
            Workbook workbook = new Workbook("example.xlsm");
            
            // Acceder al proyecto VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Obtener códigos binarios del primer módulo
            byte[] binaryCodes = vbaProject.Modules[0].BinaryCodes;
            
            // Convertir a cadena usando codificación china (936)
            string codeContent = Encoding.GetEncoding(936).GetString(binaryCodes);
            
            // Mostrar el contenido que contiene caracteres chinos
            Console.WriteLine("VBA Module Content:");
            Console.WriteLine(codeContent);
        }
    }
}
```

### Ver también

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


