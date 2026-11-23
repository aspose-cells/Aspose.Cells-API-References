---
title: "LoadOptions.StandardFont"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LoadOptions. Définit le nom de police standard par défaut"
type: docs
url: /fr/net/aspose.cells/loadoptions/standardfont/
---
## LoadOptions.StandardFont property

Définit le nom de police standard par défaut

```csharp
[Obsolete("Use DefaultStyleSettings.FontName property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StandardFont { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser DefaultStyleSettings. Cette propriété sera supprimée 12 mois plus tard à compter de mars 2022. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyStandardFontDemo
    {
        public static void Run()
        {
            // Créer un fichier Excel d'exemple en mémoire
            MemoryStream ms = new MemoryStream();
            using (Workbook workbook = new Workbook())
            {
                workbook.Worksheets[0].Cells["A1"].PutValue("Standard Font Test");
                workbook.Save(ms, SaveFormat.Xlsx);
            }
            ms.Position = 0;

            // Définir les options de chargement avec StandardFont
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.StandardFont = "SimSun";
            
            // Charger le classeur avec la police spécifiée
            Workbook workbookWithFont = new Workbook(ms, loadOptions);
            
            // Démontrer que la police est définie en vérifiant le style par défaut
            Console.WriteLine("Default font after loading: " + 
                workbookWithFont.DefaultStyle.Font.Name);
        }
    }
}
```

### Voir aussi

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


