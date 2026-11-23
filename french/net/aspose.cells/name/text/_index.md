---
title: "Name.Text"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Name. Obtient le texte du nom de l'objet"
type: docs
url: /fr/net/aspose.cells/name/text/
---
## Name.Text property

Obtient le texte du nom de l’objet.

```csharp
public string Text { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyTextDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer une plage nommée
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$B$2";
            
            // Définir et afficher la propriété Text
            namedRange.Text = "MyCustomName";
            Console.WriteLine("Named range text: " + namedRange.Text);
            
            // Enregistrez le classeur
            workbook.Save("NamedRangeExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


