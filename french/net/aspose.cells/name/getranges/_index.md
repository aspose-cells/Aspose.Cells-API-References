---
title: "Name.GetRanges"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Name. Récupère toutes les plages référencées par ce nom"
type: docs
url: /fr/net/aspose.cells/name/getranges/
---
## GetRanges() {#getranges}

Obtient toutes les plages référencées par ce nom.

```csharp
public Range[] GetRanges()
```

### Valeur de retour

Toutes les plages.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangesDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            
            // Créer une plage nommée
            int index = workbook.Worksheets.Names.Add("Fruits");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$1:$A$3";
            
            // Obtenir les plages avec recalcul
            Aspose.Cells.Range[] ranges1 = name.GetRanges();
            Console.WriteLine("Ranges with recalculation:");
            PrintRanges(ranges1);
            
            // Obtenir les plages sans recalcul
            Aspose.Cells.Range[] ranges2 = name.GetRanges(false);
            Console.WriteLine("\nRanges without recalculation:");
            PrintRanges(ranges2);
        }
        
        private static void PrintRanges(Aspose.Cells.Range[] ranges)
        {
            if (ranges != null)
            {
                foreach (Aspose.Cells.Range range in ranges)
                {
                    Console.WriteLine($"Range: {range.Address}");
                }
            }
            else
            {
                Console.WriteLine("No ranges found");
            }
        }
    }
}
```

### Voir aussi

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRanges(bool) {#getranges_1}

Obtient toutes les plages référencées par ce nom.

```csharp
public Range[] GetRanges(bool recalculate)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| recalculer | Boolean | si le recalcul doit être effectué si ce nom a déjà été calculé avant cet appel. |

### Valeur de retour

Toutes les plages.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangesWithBooleanDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            
            // Créer une plage nommée
            int index = workbook.Worksheets.Names.Add("TestRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$A$3";
            
            // Obtenir les plages sans recalculer
            Aspose.Cells.Range[] ranges1 = namedRange.GetRanges(false);
            Console.WriteLine("Ranges count (no recalc): " + ranges1.Length);
            
            // Obtenir les plages avec recalcul
            Aspose.Cells.Range[] ranges2 = namedRange.GetRanges();
            Console.WriteLine("Ranges count (with recalc): " + ranges2.Length);
            
            // Modifier la plage et démontrer le recalcul
            worksheet.Cells["A4"].PutValue(30);
            namedRange.RefersTo = "=Sheet1!$A$1:$A$4";
            
            // Obtenir les plages avec et sans recalcul après modification
            Aspose.Cells.Range[] ranges3 = namedRange.GetRanges(false);
            Console.WriteLine("Ranges count after mod (no recalc): " + ranges3.Length);
            
            Aspose.Cells.Range[] ranges4 = namedRange.GetRanges();
            Console.WriteLine("Ranges count after mod (with recalc): " + ranges4.Length);
        }
    }
}
```

### Voir aussi

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


