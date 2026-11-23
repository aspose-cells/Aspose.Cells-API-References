---
title: "PivotFilter.GetTop10Value"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotFilter. Obtient le paramètre top 10 du filtre"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfilter/gettop10value/
---
## PivotFilter.GetTop10Value method

Obtient le paramètre top 10 du filtre.

```csharp
public Top10Filter GetTop10Value()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterMethodGetTop10ValueDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accéder à la première feuille de calcul et au tableau croisé dynamique
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Appliquer un filtre top 10 sur le premier champ de base (afficher les 2 premiers éléments par nombre)
            pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
            
            // Obtenir le filtre appliqué et sa valeur top 10
            PivotFilter filter = pivotTable.BaseFields[0].GetFilters()[0];
            Top10Filter top10Filter = filter.GetTop10Value();
            
            // Afficher les détails du filtre
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Top 10 Items: " + top10Filter.Items);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Top10Filter](../../../aspose.cells/top10filter/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


