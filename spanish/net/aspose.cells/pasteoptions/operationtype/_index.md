---
title: "PasteOptions.OperationType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PasteOptions. Obtiene y establece el tipo de operación al pegar el rango"
type: docs
url: /es/net/aspose.cells/pasteoptions/operationtype/
---
## PasteOptions.OperationType property

Obtiene y establece el tipo de operación al pegar el rango.

```csharp
public PasteOperationType OperationType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyOperationTypeDemo
    {
        public static void Run()
        {
            // Cree el libro de origen con datos de ejemplo
            Workbook wbOrigin = new Workbook();
            Worksheet sourceSheet = wbOrigin.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["B2"].PutValue(100);
            
            // Cree un libro de trabajo de destino
            Workbook wbDestination = new Workbook();
            Worksheet destSheet = wbDestination.Worksheets[0];
            destSheet.Cells["A1"].PutValue("Destination Data");
            destSheet.Cells["B2"].PutValue(200); // Will be modified by paste operation
            
            // Crear rangos para copiar/pegar
            var rangeOrigin = sourceSheet.Cells.CreateRange("A1:B3");
            var rangeDestination = destSheet.Cells.CreateRange("A1:B3");
            
            // Crear opciones de pegado con demostración de OperationType
            var options = new PasteOptions
            {
                PasteType = PasteType.All,
                OperationType = PasteOperationType.Add // Values will be added (100 + 200 = 300)
            };
            
            // Ejecutar la operación de copiar/pegar
            rangeDestination.Copy(rangeOrigin, options);
            
            // Verificar el resultado
            Console.WriteLine("B2 value after paste with Add operation: " + destSheet.Cells["B2"].IntValue);
            
            // Guardar el resultado
            wbDestination.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* enum [PasteOperationType](../../pasteoperationtype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


