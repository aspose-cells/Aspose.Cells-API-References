---
title: "Enum SensitivityLabelMarkType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Metas.SensitivityLabelMarkType enum. Representerar typerna av innehållsmärkning som bör tillämpas på en fil"
type: docs
url: /sv/net/aspose.cells.metas/sensitivitylabelmarktype/
---
## SensitivityLabelMarkType enumeration

Representerar typerna av innehållsmärkning som bör tillämpas på en fil.

```csharp
[Flags]
public enum SensitivityLabelMarkType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ingen |
| Header | `1` | Sidhuvud |
| Footer | `2` | Sidfot |
| Watermark | `4` | Vattenstämpel |
| Encryption | `8` | Kryptering |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class MetasClassSensitivityLabelMarkTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Demonstrera värden för SensitivityLabelMarkType-enum
            SensitivityLabelMarkType markType = SensitivityLabelMarkType.Watermark;

            // Applicera olika känslighetsetikettmarkeringar baserat på typen
            switch (markType)
            {
                case SensitivityLabelMarkType.None:
                    Console.WriteLine("No sensitivity label applied");
                    break;
                case SensitivityLabelMarkType.Header:
                    worksheet.PageSetup.SetHeader(0, "CONFIDENTIAL");
                    break;
                case SensitivityLabelMarkType.Footer:
                    worksheet.PageSetup.SetFooter(0, "INTERNAL USE ONLY");
                    break;
                case SensitivityLabelMarkType.Watermark:
                    worksheet.PageSetup.SetHeader(0, "&KFF0000&DRAFT");
                    break;
                case SensitivityLabelMarkType.Encryption:
                    workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, 128);
                    break;
            }

            // Spara arbetsboken med applicerad känslighetsetikett
            workbook.Save("SensitivityLabelMarkTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


