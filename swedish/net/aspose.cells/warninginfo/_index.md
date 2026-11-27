---
title: "Klass WarningInfo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.WarningInfo-klass. Varningsinformation"
type: docs
url: /sv/net/aspose.cells/warninginfo/
---
## WarningInfo class

Varningsinformation

```csharp
public class WarningInfo
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CorrectedObject](../../aspose.cells/warninginfo/correctedobject/) { get; set; } | Hämtar och anger det korrigerade objektet. |
| [Description](../../aspose.cells/warninginfo/description/) { get; } | Hämta beskrivning av varningsinformation. |
| [ErrorObject](../../aspose.cells/warninginfo/errorobject/) { get; } | Felobjektet. |
| [Type](../../aspose.cells/warninginfo/type/) { get; } | Hämta varningstyp. |
| [WarningType](../../aspose.cells/warninginfo/warningtype/) { get; } | (**Obsolete.**) Hämta varningstyp. |

### Exempel

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

            // Ställ in varningsåteranrop
            workbook.Settings.WarningCallback = new WarningHandler();

            // Utlösa olika varningstyper
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

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


