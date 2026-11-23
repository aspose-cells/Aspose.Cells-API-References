---
title: "WorkbookSettings.MemorySetting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient ou définit les options d'utilisation de la mémoire. La nouvelle option sera prise comme option par défaut pour les feuilles de calcul nouvellement créées mais ne s'appliquera pas aux feuilles de calcul existantes"
type: docs
url: /fr/net/aspose.cells/workbooksettings/memorysetting/
---
## WorkbookSettings.MemorySetting property

Obtient ou définit les options d'utilisation de la mémoire. La nouvelle option sera prise comme option par défaut pour les feuilles de calcul nouvellement créées mais ne prendra pas effet pour les feuilles de calcul existantes.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Remarques

Pour plus de détails sur le mode mémoire, veuillez consulter [`MemorySetting`](../../cells/memorysetting/).

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMemorySettingDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec le paramètre de préférence mémoire
            Workbook wb = new Workbook();
            wb.Settings.MemorySetting = MemorySetting.MemoryPreference;
            
            // Accédez à la première feuille de calcul et ajoutez des données
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Memory Setting Demo");
            sheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            
            // Enregistrer dans un flux mémoire au format PDF
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Pdf);
                Console.WriteLine("Workbook saved to PDF with MemoryPreference setting");
            }
        }
    }
}
```

### Voir aussi

* enum [MemorySetting](../../memorysetting/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


