---
title: "TableStyleCollection.DefaultTableStyleName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TableStyleCollection. Obtient et définit le nom du style par défaut du tableau"
type: docs
url: /fr/net/aspose.cells.tables/tablestylecollection/defaulttablestylename/
---
## TableStyleCollection.DefaultTableStyleName property

Obtient et définit le nom du style par défaut du tableau.

```csharp
public string DefaultTableStyleName { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleCollectionPropertyDefaultTableStyleNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez à la collection des styles de tableau
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            
            // Afficher le nom du style de tableau par défaut
            Console.WriteLine("Default Table Style: " + tableStyles.DefaultTableStyleName);
            
            // Modifie le style de tableau par défaut
            tableStyles.DefaultTableStyleName = "TableStyleMedium9";
            Console.WriteLine("New Default Table Style: " + tableStyles.DefaultTableStyleName);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


