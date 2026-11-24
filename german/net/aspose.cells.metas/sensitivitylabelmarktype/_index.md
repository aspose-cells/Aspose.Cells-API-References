---
title: "Enum SensitivityLabelMarkType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Metas.SensitivityLabelMarkType enum. Stellt die Arten der Inhaltskennzeichnung dar, die auf eine Datei angewendet werden sollen."
type: docs
url: /de/net/aspose.cells.metas/sensitivitylabelmarktype/
---
## SensitivityLabelMarkType enumeration

Stellt die Arten der Inhaltskennzeichnung dar, die auf eine Datei angewendet werden sollten.

```csharp
[Flags]
public enum SensitivityLabelMarkType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Keine |
| Header | `1` | Kopfzeile |
| Footer | `2` | Fußzeile |
| Watermark | `4` | Wasserzeichen |
| Encryption | `8` | Verschlüsselung |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Demonstriere die Werte des Enums SensitivityLabelMarkType
            SensitivityLabelMarkType markType = SensitivityLabelMarkType.Watermark;

            // Wende verschiedene Sensitivitätskennzeichen basierend auf dem Typ an
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

            // Speichere die Arbeitsmappe mit angewendetem Sensitivitätslabel
            workbook.Save("SensitivityLabelMarkTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


