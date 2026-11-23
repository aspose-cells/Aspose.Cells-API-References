---
title: "OleObject.IsLink"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OleObject. Retourne true si l'OleObject est lié au fichier"
type: docs
url: /fr/net/aspose.cells.drawing/oleobject/islink/
---
## OleObject.IsLink property

Renvoie vrai si l'OleObject est lié au fichier.

```csharp
public bool IsLink { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyIsLinkDemo
    {
        public static void Run()
        {
            // Charger le classeur source
            Workbook workbook = new Workbook("example.xlsm");

            // Traiter chaque feuille de calcul
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                // Traiter chaque objet OLE dans la feuille de calcul
                foreach (Aspose.Cells.Drawing.OleObject ole in worksheet.OleObjects)
                {
                    // Ignorer si l'objet OLE n'est pas lié
                    if (!ole.IsLink)
                    {
                        Console.WriteLine("Skipping embedded OLE object");
                        continue;
                    }

                    // Afficher et modifier le chemin du fichier lié
                    Console.WriteLine("Original linked file: " + ole.ObjectSourceFullName);
                    string newPath = ole.ObjectSourceFullName.Replace("C:", "D:");
                    ole.ObjectSourceFullName = newPath;
                    Console.WriteLine("Modified linked file: " + ole.ObjectSourceFullName);
                }
            }

            // Enregistrer le classeur modifié
            workbook.Save("modified_example.xlsm");
            Console.WriteLine("File saved with updated OLE links.");
        }
    }
}
```

### Voir aussi

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


