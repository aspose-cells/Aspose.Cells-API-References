---
title: "HorizontalPageBreakCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HorizontalPageBreakCollection. Obtient l'élément HorizontalPageBreak à l'index spécifié"
type: docs
url: /fr/net/aspose.cells/horizontalpagebreakcollection/item/
---
## HorizontalPageBreakCollection indexer (1 of 2)

Obtient l'élément [`HorizontalPageBreak`](../../horizontalpagebreak/) à l'index spécifié.

```csharp
public HorizontalPageBreak this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice à base zéro de l'élément. |

### Valeur de retour

L’élément à l’index spécifié.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des ruptures de page horizontales
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            
            // Accéder aux sauts de page en utilisant la propriété Item
            HorizontalPageBreak firstBreak = worksheet.HorizontalPageBreaks[0];
            Console.WriteLine("First page break row: " + firstBreak.Row);
            
            // Modifier les cellules qui affectent les sauts de page
            worksheet.Cells.DeleteRows(0, 2);
            
            // Vérifier que le saut de page a été ajusté
            Console.WriteLine("First page break after row deletion: " + worksheet.HorizontalPageBreaks[0].Row);
        }
    }
}
```

### Voir aussi

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HorizontalPageBreakCollection indexer (2 of 2)

Récupère l'élément [`HorizontalPageBreak`](../../horizontalpagebreak/) avec le nom de cellule spécifié.

```csharp
public HorizontalPageBreak this[string cellName] { get; }
```

| Paramètre | Description |
| --- | --- |
| cellName | Nom de la cellule. |

### Valeur de retour

L'élément avec le nom de cellule spécifié.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;

    public class HorizontalPageBreakCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajouter quelques sauts de page horizontaux en utilisant différentes surcharges
                worksheet.HorizontalPageBreaks.Add(5);          // break after row index 5
                worksheet.HorizontalPageBreaks.Add("D5");      // break at cell D5 (row index 4)

                // ----- Accès via un indice entier (Item[int]) -----
                // La propriété Item est l'indexeur, donc nous utilisons la syntaxe []
                HorizontalPageBreak firstBreak = worksheet.HorizontalPageBreaks[0];
                Console.WriteLine("First break row (int index): " + firstBreak.Row);

                // ----- Accès via une clé de chaîne (Item[string]) -----
                // Récupérer le saut de page qui a été ajouté avec le nom de cellule "D5"
                HorizontalPageBreak breakByCell = worksheet.HorizontalPageBreaks["D5"];
                Console.WriteLine("Break added with \"D5\" is at row: " + breakByCell.Row);

                // Enregistrer le classeur pour vérifier que les sauts de page sont persistés
                workbook.Save("HorizontalPageBreaks_ItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


