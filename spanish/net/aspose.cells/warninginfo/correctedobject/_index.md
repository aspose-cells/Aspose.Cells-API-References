---
title: "WarningInfo.CorrectedObject"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WarningInfo. Obtiene y establece el objeto corregido"
type: docs
url: /es/net/aspose.cells/warninginfo/correctedobject/
---
## WarningInfo.CorrectedObject property

Obtiene y establece el objeto corregido.

```csharp
public object CorrectedObject { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyCorrectedObjectDemo
    {
        public static void Run()
        {
            // Cree un libro de trabajo y genere una advertencia
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establece un nombre que normalmente activaría una advertencia
            string originalName = "MyRange";
            worksheet.Cells.CreateRange(originalName);
            
            // Manejar la devolución de llamada de advertencia
            workbook.Settings.WarningCallback = new WarningHandler();
            
            // Esta operación activaría la devolución de llamada de advertencia
            worksheet.Cells.CreateRange(originalName); // Duplicate range name
        }
    }

    public class WarningHandler : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            if (warningInfo.WarningType == WarningType.DuplicateDefinedName)
            {
                // Demostrar el uso de CorrectedObject
                warningInfo.CorrectedObject = "_" + warningInfo.ErrorObject;
                Console.WriteLine($"Warning handled. Original: {warningInfo.ErrorObject}, Corrected: {warningInfo.CorrectedObject}");
            }
        }
    }
}
```

### Ver también

* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


