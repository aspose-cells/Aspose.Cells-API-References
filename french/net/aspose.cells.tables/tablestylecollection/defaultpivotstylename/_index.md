---
title: "TableStyleCollection.DefaultPivotStyleName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TableStyleCollection. Obtient et définit le nom du style par défaut du tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.tables/tablestylecollection/defaultpivotstylename/
---
## TableStyleCollection.DefaultPivotStyleName property

Obtient et définit le nom du style par défaut de la table pivot.

```csharp
public string DefaultPivotStyleName { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleCollectionPropertyDefaultPivotStyleNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez à la collection des styles de tableau
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            
            // Afficher le nom du style par défaut du tableau croisé dynamique
            Console.WriteLine("Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
            
            // Modifier le style par défaut du tableau croisé dynamique
            tableStyles.DefaultPivotStyleName = "PivotStyleDark2";
            
            // Vérifier le changement
            Console.WriteLine("Updated Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
            
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


