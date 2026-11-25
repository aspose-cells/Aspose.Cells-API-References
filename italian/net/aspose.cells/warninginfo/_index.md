---
title: "Classe WarningInfo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.WarningInfo. Informazioni di avviso"
type: docs
url: /it/net/aspose.cells/warninginfo/
---
## WarningInfo class

Informazioni di avviso

```csharp
public class WarningInfo
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CorrectedObject](../../aspose.cells/warninginfo/correctedobject/) { get; set; } | Ottiene e imposta l'oggetto corretto. |
| [Description](../../aspose.cells/warninginfo/description/) { get; } | Ottieni la descrizione delle informazioni di avviso. |
| [ErrorObject](../../aspose.cells/warninginfo/errorobject/) { get; } | L'oggetto errore. |
| [Type](../../aspose.cells/warninginfo/type/) { get; } | Ottieni il tipo di avviso. |
| [WarningType](../../aspose.cells/warninginfo/warningtype/) { get; } | (**Obsolete.**) Ottieni il tipo di avviso. |

### Esempi

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

            // Imposta la callback di avviso
            workbook.Settings.WarningCallback = new WarningHandler();

            // Attiva diversi tipi di avviso
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

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


