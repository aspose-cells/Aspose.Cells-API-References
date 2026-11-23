---
title: "Énum SensitivityLabelMarkType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Metas.SensitivityLabelMarkType enum. Représente les types de marquage de contenu qui doivent être appliqués à un fichier"
type: docs
url: /fr/net/aspose.cells.metas/sensitivitylabelmarktype/
---
## SensitivityLabelMarkType enumeration

Représente les types de marquage de contenu qui doivent être appliqués à un fichier.

```csharp
[Flags]
public enum SensitivityLabelMarkType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Aucun |
| Header | `1` | En-tête |
| Footer | `2` | Pied de page |
| Watermark | `4` | Filigrane |
| Encryption | `8` | Chiffrement |

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Démontrez les valeurs de l'énum SensitivityLabelMarkType
            SensitivityLabelMarkType markType = SensitivityLabelMarkType.Watermark;

            // Appliquez différents marquages de label de sensibilité en fonction du type
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

            // Enregistrez le classeur avec le label de sensibilité appliqué
            workbook.Save("SensitivityLabelMarkTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


