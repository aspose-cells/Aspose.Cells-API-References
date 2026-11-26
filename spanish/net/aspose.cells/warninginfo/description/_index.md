---
title: "WarningInfo.Description"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WarningInfo. Obtenga la descripción de la información de advertencia"
type: docs
url: /es/net/aspose.cells/warninginfo/description/
---
## WarningInfo.Description property

Obtén la descripción de la información de advertencia.

```csharp
public string Description { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyDescriptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree un nombre definido duplicado para generar una advertencia
            worksheet.Cells.CreateRange(0, 0, 10, 10).Name = "_XLNM.PRINT_AREA";
            worksheet.Cells.CreateRange(0, 0, 10, 10).Name = "_XLNM.PRINT_AREA"; // Different name to actually trigger warning

            // Obtener la devolución de llamada de advertencia
            WarningCallback callback = new WarningCallback();
            workbook.Settings.WarningCallback = callback; // Correct property path

            // Guardar para generar una advertencia
            workbook.Save("output.xlsx");

            // Demostrar el uso de la propiedad Description
            if (callback.LastWarning != null)
            {
                Console.WriteLine("Warning Description: " + callback.LastWarning.Description);
                Console.WriteLine("Warning Type: " + callback.LastWarning.Type);
            }
        }
    }

    public class WarningCallback : IWarningCallback
    {
        public WarningInfo LastWarning { get; private set; }

        public void Warning(WarningInfo warningInfo)
        {
            LastWarning = warningInfo;
        }
    }
}
```

### Ver también

* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


