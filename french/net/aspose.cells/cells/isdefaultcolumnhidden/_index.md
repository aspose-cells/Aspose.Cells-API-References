---
title: "Cells.IsDefaultColumnHidden"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells."
type: docs
url: /fr/net/aspose.cells/cells/isdefaultcolumnhidden/
---
## Cells.IsDefaultColumnHidden property

```csharp
public bool IsDefaultColumnHidden { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyIsDefaultColumnHiddenDemo
    {
        public static void Run()
        {
            try
            {
                // Créez un nouveau classeur et obtenez la première feuille de calcul
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Ajoutez des données afin que la feuille de calcul ne soit pas vide
                cells["A1"].PutValue("First");
                cells["B1"].PutValue("Second");
                cells["C1"].PutValue("Third");

                // Lire la propriété IsDefaultColumnHidden (la valeur par défaut est false)
                bool isDefaultColumnHidden = cells.IsDefaultColumnHidden;
                Console.WriteLine("IsDefaultColumnHidden: " + isDefaultColumnHidden);

                // Enregistrez le classeur (optionnel, juste pour compléter la démonstration)
                workbook.Save("IsDefaultColumnHiddenDemo.xlsx", SaveFormat.Xlsx);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


