---
title: "Enum EmfRenderSetting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.EmfRenderSetting. Paramètre pour le rendu du métafichier Emf"
type: docs
url: /fr/net/aspose.cells/emfrendersetting/
---
## EmfRenderSetting enumeration

Paramètre pour le rendu du métafichier Emf.

```csharp
public enum EmfRenderSetting
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| EmfOnly | `0` | Rendu uniquement des enregistrements Emf. |
| EmfPlusPrefer | `1` | Préférer le rendu des enregistrements EmfPlus. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class CellsClassEmfRenderSettingDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("EMF Render Setting Demo");
            worksheet.Cells["A2"].PutValue("Using EmfOnly setting");

            // Créer des options d'image avec le paramètre de rendu EMF
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                EmfRenderSetting = EmfRenderSetting.EmfOnly
            };

            // Créer un rendu de feuille avec les options
            SheetRender render = new SheetRender(worksheet, options);

            // Enregistrer la première page en tant qu'image EMF
            render.ToImage(0, "EmfRenderSettingDemo.emf");

            Console.WriteLine("EMF file created successfully with EmfOnly setting.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


