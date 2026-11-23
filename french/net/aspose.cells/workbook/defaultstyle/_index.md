---
title: "Workbook.DefaultStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Obtient ou définit l'objet Style par défaut du classeur"
type: docs
url: /fr/net/aspose.cells/workbook/defaultstyle/
---
## Workbook.DefaultStyle property

Obtient ou définit l'objet [`Style`](../../style/) par défaut du classeur.

```csharp
public Style DefaultStyle { get; set; }
```

### Remarques

La propriété DefaultStyle est utile pour appliquer un Style à l'ensemble du classeur.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyDefaultStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Obtenez le style par défaut et modifiez sa police
            Style defaultStyle = workbook.DefaultStyle;
            defaultStyle.Font.Name = "Tahoma";
            defaultStyle.Font.Size = 12;
            
            // Appliquez le style modifié à nouveau comme style par défaut
            workbook.DefaultStyle = defaultStyle;
            
            // Créez une feuille de calcul et ajoutez du texte avec le style par défaut
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This text uses the default Tahoma font");
            
            // Enregistrez le classeur
            workbook.Save("DefaultStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


