---
title: "Workbook.IsLicensed"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Workbook property. Indica si la licencia está establecida"
type: docs
url: /es/net/aspose.cells/workbook/islicensed/
---
## Workbook.IsLicensed property

Indica si la licencia está establecida.

```csharp
public bool IsLicensed { get; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsLicensedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            
            // Establecer algunas propiedades básicas para demostrar que el libro de trabajo está siendo usado
            wb.Worksheets[0].Name = "Sheet1";
            wb.Worksheets[0].Cells[0, 0].PutValue("Sample Data");
            
            // Verificar si el libro de trabajo está licenciado
            Console.WriteLine($"IsLicensed: {wb.IsLicensed}");
            
            // Demostrar un comportamiento diferente según el estado de la licencia
            if (wb.IsLicensed)
            {
                Console.WriteLine("Running in licensed mode - full features available");
            }
            else
            {
                Console.WriteLine("Running in evaluation mode - watermarks will appear");
            }

            // Guardar en un flujo de memoria para demostrar la funcionalidad
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
                Console.WriteLine($"Workbook saved successfully (Size: {ms.Length} bytes)");
            }
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


