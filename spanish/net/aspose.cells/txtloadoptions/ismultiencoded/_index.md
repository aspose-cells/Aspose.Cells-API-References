---
title: "TxtLoadOptions.IsMultiEncoded"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtLoadOptions. True indica que el archivo contiene varias codificaciones"
type: docs
url: /es/net/aspose.cells/txtloadoptions/ismultiencoded/
---
## TxtLoadOptions.IsMultiEncoded property

Verdadero indica que el archivo contiene varias codificaciones.

```csharp
public bool IsMultiEncoded { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyIsMultiEncodedDemo
    {
        public static void Run()
        {
            // Crea opciones de carga de texto
            TxtLoadOptions options = new TxtLoadOptions();
            
            // Establezca IsMultiEncoded a true para manejar múltiples codificaciones
            options.IsMultiEncoded = true;
            
            // Cargue el libro de trabajo con las opciones
            Workbook workbook = new Workbook("example.csv", options);
            
            // Muestre valores de muestra del archivo cargado
            Console.WriteLine("A2 Cell Value: " + workbook.Worksheets[0].Cells["A2"].StringValue);
            Console.WriteLine("A3 Cell Value: " + workbook.Worksheets[0].Cells["A3"].StringValue);
        }
    }
}
```

### Ver también

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


