---
title: "AutoFilter.RemoveFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AutoFilter. Supprime un filtre pour une colonne de filtre"
type: docs
url: /fr/net/aspose.cells/autofilter/removefilter/
---
## RemoveFilter(int, string) {#removefilter_1}

Supprime un filtre pour une colonne de filtre.

```csharp
public void RemoveFilter(int fieldIndex, string criteria)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |
| critères | String | Le critère spécifié (une chaîne ; par exemple, "101"). Il ne peut être nul ou être l'une des valeurs des cellules de cette colonne. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodRemoveFilterWithInt32StringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir des données d'exemple pour la démonstration
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["C1"].PutValue("Price");
            
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue("Electronics");
            worksheet.Cells["C2"].PutValue(999.99);
            
            worksheet.Cells["A3"].PutValue("Novel");
            worksheet.Cells["B3"].PutValue("Books");
            worksheet.Cells["C3"].PutValue(19.99);
            
            worksheet.Cells["A4"].PutValue("Smartphone");
            worksheet.Cells["B4"].PutValue("Electronics");
            worksheet.Cells["C4"].PutValue(599.99);

            // Définir la plage du filtre automatique (en-têtes + 3 lignes de données)
            worksheet.AutoFilter.SetRange(0, 0, 2);

            try
            {
                AutoFilter autoFilter = worksheet.AutoFilter;
                
                // Appliquer un filtre sur la colonne Catégorie (fieldIndex 1) pour "Électronique"
                autoFilter.AddFilter(1, "Electronics");
                autoFilter.Refresh(); // Apply filter to hide non-matching rows
                
                // Supprimer le filtre spécifique de la colonne Catégorie
                autoFilter.RemoveFilter(1, "Electronics");
                autoFilter.Refresh(); // Re-apply filter (now shows all rows)

                Console.WriteLine("RemoveFilter executed: Electronics filter removed from Category column.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Enregistrer le classeur modifié
            workbook.Save("AutoFilterMethodRemoveFilterWithInt32StringDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveFilter(int) {#removefilter}

Supprime le filtre spécifique.

```csharp
public void RemoveFilter(int fieldIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | L'index du filtre spécifique |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRemoveFilterWithInt32Demo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Grape");
            
            // Appliquer le filtre automatique
            worksheet.AutoFilter.Range = "A1:A5";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Ajouter un filtre
            filter.AddFilter(0, "Apple");
            filter.Refresh();
            
            Console.WriteLine("After adding filter - Visible rows:");
            PrintVisibleRows(worksheet);
            
            // Supprimer le filtre
            filter.RemoveFilter(0);
            filter.Refresh();
            
            Console.WriteLine("\nAfter removing filter - Visible rows:");
            PrintVisibleRows(worksheet);
        }
        
        private static void PrintVisibleRows(Worksheet worksheet)
        {
            for (int i = 0; i < worksheet.Cells.MaxDataRow + 1; i++)
            {
                if (!worksheet.Cells.Rows[i].IsHidden)
                {
                    Console.WriteLine($"Row {i + 1}: {worksheet.Cells[i, 0].StringValue}");
                }
            }
        }
    }
}
```

### Voir aussi

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


