---
title: "Énum MemorySetting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.MemorySetting enum. Modes d'utilisation de la mémoire pour le modèle de données des cellules"
type: docs
url: /fr/net/aspose.cells/memorysetting/
---
## MemorySetting enumeration

Modes d'utilisation de la mémoire pour le modèle de données des cellules.

```csharp
public enum MemorySetting
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Normal | `0` | Mode par défaut pour le modèle de cellules. |
| MemoryPreference | `1` | Performance mémoire préférable. |
| FileCache | `2` | Performance mémoire préférable et utilisation d'un fichier au lieu de la mémoire pour conserver les données des cellules. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MemorySettingDemo
    {
        public static void MemorySettingExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder aux paramètres du classeur
            WorkbookSettings settings = workbook.Settings;

            // Définissez l'option d'utilisation de la mémoire sur MemoryPreference
            settings.MemorySetting = MemorySetting.MemoryPreference;

            // Créez une feuille de calcul et ajoutez des données
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);

            // Enregistrez le classeur
            workbook.Save("MemorySettingExample.xlsx");

            Console.WriteLine("Workbook saved with MemorySetting.MemoryPreference.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


