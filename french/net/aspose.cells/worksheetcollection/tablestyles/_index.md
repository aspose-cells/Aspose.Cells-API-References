---
title: "WorksheetCollection.TableStyles"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorksheetCollection. Obtient l'objet TableStyles"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/tablestyles/
---
## WorksheetCollection.TableStyles property

Obtient l'objet `TableStyles`.

```csharp
public TableStyleCollection TableStyles { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyTableStylesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter plusieurs feuilles de calcul
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            
            // Créer et ajouter des styles de tableau
            int styleIndex1 = workbook.Worksheets.TableStyles.AddTableStyle("Style1");
            TableStyle style1 = workbook.Worksheets.TableStyles[styleIndex1];
            
            int styleIndex2 = workbook.Worksheets.TableStyles.AddTableStyle("Style2");
            TableStyle style2 = workbook.Worksheets.TableStyles[styleIndex2];
            
            // Afficher le nombre de styles de tableau
            Console.WriteLine("Table styles count: " + workbook.Worksheets.TableStyles.Count);
            
            // Supprimer un style
            workbook.Worksheets.TableStyles.RemoveAt(0);
            
            // Afficher le nombre mis à jour
            Console.WriteLine("Table styles count after removal: " + workbook.Worksheets.TableStyles.Count);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [TableStyleCollection](../../../aspose.cells.tables/tablestylecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


