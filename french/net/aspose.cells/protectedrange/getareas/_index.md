---
title: "ProtectedRange.GetAreas"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ProtectedRange method. Obtient toutes les zones référencées"
type: docs
url: /fr/net/aspose.cells/protectedrange/getareas/
---
## ProtectedRange.GetAreas method

Obtient toutes les zones référencées.

```csharp
public CellArea[] GetAreas()
```

### Valeur de retour

Renvoie toutes les zones référencées.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangeMethodGetAreasDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenir la collection de plages protégées
            ProtectedRangeCollection protectedRanges = worksheet.AllowEditRanges;
            
            // Ajouter une plage protégée
            int index = protectedRanges.Add("TestRange", 0, 0, 10, 10);
            ProtectedRange protectedRange = protectedRanges[index];
            
            // Obtenir les zones de la plage protégée
            CellArea[] areas = protectedRange.GetAreas();
            
            // Afficher le nombre de zones (devrait être 1 pour cette plage simple)
            Console.WriteLine("Number of areas in protected range: " + areas.Length);
            
            // Enregistrez le classeur
            workbook.Save("ProtectedRangeExample.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


