---
title: "Enum SensitivityLabelMarkType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Metas.SensitivityLabelMarkType enum. Rappresenta i tipi di marcatura del contenuto che dovrebbero essere applicati a un file"
type: docs
url: /it/net/aspose.cells.metas/sensitivitylabelmarktype/
---
## SensitivityLabelMarkType enumeration

Rappresenta i tipi di marcatura del contenuto che dovrebbero essere applicati a un file.

```csharp
[Flags]
public enum SensitivityLabelMarkType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessuno |
| Header | `1` | Intestazione |
| Footer | `2` | Piè di pagina |
| Watermark | `4` | Filigrana |
| Encryption | `8` | Crittografia |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dimostra i valori dell'enum SensitivityLabelMarkType
            SensitivityLabelMarkType markType = SensitivityLabelMarkType.Watermark;

            // Applica diverse marcature dell'etichetta di sensibilità in base al tipo
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

            // Salva la cartella di lavoro con l'etichetta di sensibilità applicata
            workbook.Save("SensitivityLabelMarkTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


