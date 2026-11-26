---
title: "Clase WarningInfo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.WarningInfo. Información de advertencia"
type: docs
url: /es/net/aspose.cells/warninginfo/
---
## WarningInfo class

Información de advertencia

```csharp
public class WarningInfo
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CorrectedObject](../../aspose.cells/warninginfo/correctedobject/) { get; set; } | Obtiene y establece el objeto corregido. |
| [Description](../../aspose.cells/warninginfo/description/) { get; } | Obtén la descripción de la información de advertencia. |
| [ErrorObject](../../aspose.cells/warninginfo/errorobject/) { get; } | El objeto de error. |
| [Type](../../aspose.cells/warninginfo/type/) { get; } | Obtener tipo de advertencia. |
| [WarningType](../../aspose.cells/warninginfo/warningtype/) { get; } | (**Obsolete.**) Obtener tipo de advertencia. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassWarningInfoDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer devolución de llamada de advertencia
            workbook.Settings.WarningCallback = new WarningHandler();

            // Activar diferentes tipos de advertencia
            worksheet.Cells["A1"].PutValue("InvalidName"); // Will trigger DefinedName warning
            worksheet.Cells["A2"].PutValue(DateTime.MaxValue); // May trigger other warnings

            Console.WriteLine("Warning demo completed.");
        }
    }

    public class WarningHandler : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            switch (warningInfo.WarningType)
            {
                case WarningType.DuplicateDefinedName:
                    warningInfo.CorrectedObject = "_" + warningInfo.ErrorObject;
                    Console.WriteLine($"DefinedName warning handled. Corrected to: {warningInfo.CorrectedObject}");
                    break;
                case WarningType.FontSubstitution:
                    Console.WriteLine($"Font warning: {warningInfo.Description}");
                    break;
                case WarningType.UnsupportedFileFormat:
                    Console.WriteLine($"File format warning: {warningInfo.Description}");
                    break;
                case WarningType.IO:
                    Console.WriteLine($"IO warning: {warningInfo.Description}");
                    break;
                case WarningType.InvalidData:
                case WarningType.Limitation:
                    Console.WriteLine($"Warning: {warningInfo.Description}");
                    break;
                default:
                    Console.WriteLine($"Unknown warning type: {warningInfo.Description}");
                    break;
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


