---
title: "HtmlSaveOptions.IsFullPathLink"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si l'on utilise un lien de chemin complet dans sheet00x.htmfilelist.xml et tabstrip.htm. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/isfullpathlink/
---
## HtmlSaveOptions.IsFullPathLink property

Indique s’il faut utiliser un lien avec chemin complet dans sheet00x.htm, filelist.xml et tabstrip.htm. La valeur par défaut est false.

```csharp
public bool IsFullPathLink { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsFullPathLinkDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test HTML Export");

            // Créer des options d'enregistrement HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Démontrer la propriété IsFullPathLink
            saveOptions.IsFullPathLink = true; // Set to true to use full path links
            
            // Enregistrer avec différents paramètres IsFullPathLink
            workbook.Save("HtmlExport_FullPathLinks.html", saveOptions);
            
            saveOptions.IsFullPathLink = false; // Set to false for relative paths
            workbook.Save("HtmlExport_RelativeLinks.html", saveOptions);
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


