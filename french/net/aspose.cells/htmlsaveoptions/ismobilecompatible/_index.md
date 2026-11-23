---
title: "HtmlSaveOptions.IsMobileCompatible"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si le HTML de sortie est compatible avec les appareils mobiles. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/ismobilecompatible/
---
## HtmlSaveOptions.IsMobileCompatible property

Indique si le HTML généré est compatible avec les appareils mobiles. La valeur par défaut est false.

```csharp
public bool IsMobileCompatible { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsMobileCompatibleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Mobile Compatibility Test");

            // Créer des options d'enregistrement HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Définir la compatibilité mobile
            saveOptions.IsMobileCompatible = true;

            // Enregistrer avec la compatibilité mobile activée
            workbook.Save("MobileCompatible.html", saveOptions);

            // Passer à non compatible mobile
            saveOptions.IsMobileCompatible = false;
            workbook.Save("NonMobileCompatible.html", saveOptions);
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


