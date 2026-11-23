---
title: "Classe LowCodeLoadOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.LowCode.LowCodeLoadOptions. Options pour charger le fichier modèle"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodeloadoptions/
---
## LowCodeLoadOptions class

Options pour charger le fichier de modèle.

```csharp
public class LowCodeLoadOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [LowCodeLoadOptions](lowcodeloadoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [InputFile](../../aspose.cells.lowcode/lowcodeloadoptions/inputfile/) { get; set; } | Obtient et définit le fichier (avec le chemin si nécessaire) du modèle. |
| [InputStream](../../aspose.cells.lowcode/lowcodeloadoptions/inputstream/) { get; set; } | Obtient et définit le flux du modèle. |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodeLoadOptionsDemo
    {
        public static void Run()
        {
            // Créer un flux d'exemple (en mémoire à des fins de démonstration)
            using (MemoryStream stream = new MemoryStream())
            {
                // Créer un nouveau classeur et l'enregistrer dans le flux pour la démonstration
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Save(stream, SaveFormat.Xlsx);

                // Réinitialiser la position du flux
                stream.Position = 0;

                // Créer et utiliser LowCodeLoadOptions
                var loadOptions = new LowCodeLoadOptions()
                {
                    InputStream = stream
                };

                // Exemple d'utilisation – serait généralement passé à une méthode de traitement
                Console.WriteLine($"Loading with LowCode options from stream of length: {loadOptions.InputStream.Length}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


