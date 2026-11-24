---
title: "Klasse WarningInfo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.WarningInfo Klasse. Warnungsinfo"
type: docs
url: /de/net/aspose.cells/warninginfo/
---
## WarningInfo class

Warnungsinfo

```csharp
public class WarningInfo
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CorrectedObject](../../aspose.cells/warninginfo/correctedobject/) { get; set; } | Liest und setzt das korrigierte Objekt. |
| [Description](../../aspose.cells/warninginfo/description/) { get; } | Beschreibung der Warnungsinfo abrufen. |
| [ErrorObject](../../aspose.cells/warninginfo/errorobject/) { get; } | Das Fehlerobjekt. |
| [Type](../../aspose.cells/warninginfo/type/) { get; } | Warnungstyp abrufen. |
| [WarningType](../../aspose.cells/warninginfo/warningtype/) { get; } | (**Obsolete.**) Warnungstyp abrufen. |

### Beispiele

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

            // Warnungs-Callback festlegen
            workbook.Settings.WarningCallback = new WarningHandler();

            // Verschiedene Warnungstypen auslösen
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

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


