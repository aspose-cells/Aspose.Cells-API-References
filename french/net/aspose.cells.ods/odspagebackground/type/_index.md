---
title: "OdsPageBackground.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OdsPageBackground. Obtient et définit le type d'arrière-plan de la page"
type: docs
url: /fr/net/aspose.cells.ods/odspagebackground/type/
---
## OdsPageBackground.Type property

Obtient et définit le type d'arrière-plan de la page.

```csharp
public OdsPageBackgroundType Type { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez à la configuration de page de la première feuille de calcul
            PageSetup ps = workbook.Worksheets[0].PageSetup;
            
            // Obtenez l'arrière-plan de la page ODS
            OdsPageBackground background = ps.ODSPageBackground;
            
            // Définissez le type d'arrière-plan sur graphique et configurez-le
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicData = File.ReadAllBytes("image1.png");
            background.GraphicType = OdsPageBackgroundGraphicType.Area;
            
            // Enregistrez le classeur
            workbook.Save("output.ods");
            
            // Rechargez le fichier enregistré pour vérifier les paramètres
            Workbook verifyWorkbook = new Workbook("output.ods");
            PageSetup verifyPs = verifyWorkbook.Worksheets[0].PageSetup;
            OdsPageBackground verifyBackground = verifyPs.ODSPageBackground;
            
            // Affichez les résultats de la vérification
            Console.WriteLine("Background Type: " + verifyBackground.Type);
            Console.WriteLine("Graphic Type: " + verifyBackground.GraphicType);
        }
    }
}
```

### Voir aussi

* enum [OdsPageBackgroundType](../../odspagebackgroundtype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


