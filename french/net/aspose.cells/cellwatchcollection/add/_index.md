---
title: "CellWatchCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CellWatchCollection. Ajoute un CellWatch avec une ligne et une colonne"
type: docs
url: /fr/net/aspose.cells/cellwatchcollection/add/
---
## Add(int, int) {#add}

Ajoute [`CellWatch`](../../cellwatch/) avec une ligne et une colonne.

```csharp
public int Add(int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | L'index de ligne. |
| column | Int32 | L'index de colonne. |

### Valeur de retour

Renvoie la position de cet élément dans la collection.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenez la CellWatchCollection depuis la feuille de calcul
            CellWatchCollection cellWatchCollection = worksheet.CellWatches;
            
            try
            {
                // Appelez la méthode Add avec les indices de ligne et de colonne (Int32, Int32)
                int index = cellWatchCollection.Add(5, 3); // Adding cell at row 6, column D (0-based)
                
                Console.WriteLine($"CellWatch added at index: {index}");
                
                // Vérifiez le cell watch ajouté
                CellWatch cellWatch = cellWatchCollection[index];
                Console.WriteLine($"Watching cell: {cellWatch.Row},{cellWatch.Column}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("CellWatchCollectionMethodAddWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Ajoute [`CellWatch`](../../cellwatch/) avec le nom de la cellule.

```csharp
public int Add(string cellName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | String | Le nom de la cellule. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des surveillances de cellules
            worksheet.CellWatches.Add("A1");
            worksheet.CellWatches.Add("B2");
            worksheet.CellWatches.Add("C3");
            
            // Affiche le nombre de cell watches
            Console.WriteLine("Cell Watches Count: " + worksheet.CellWatches.Count);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


