---
title: "Cells.Find"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Trouve la cellule contenant l'objet d'entrée"
type: docs
url: /fr/net/aspose.cells/cells/find/
---
## Find(object, Cell) {#find}

Trouve la cellule contenant l'objet d'entrée.

```csharp
public Cell Find(object what, Cell previousCell)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| quoi | Object | L'objet à rechercher. Le type doit être int,double,DateTime,string,bool. |
| previousCell | Cellule | Cellule précédente avec le même objet. Ce paramètre peut être défini sur null si la recherche commence depuis le début. |

### Valeur de retour

Objet Cell.

### Remarques

Renvoie null (Nothing) si aucune cellule n'est trouvée.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodFindWithObjectCellDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(1.2);

            // Trouver la cellule contenant "Orange"
            Cell searchCell = null;
            Cell foundCell = worksheet.Cells.Find("Orange", searchCell);

            if (foundCell != null)
            {
                Console.WriteLine("Found 'Orange' at: " + foundCell.Name);
                
                // Créer et appliquer un style à la cellule trouvée
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Red;
                style.Font.IsBold = true;
                foundCell.SetStyle(style);
            }

            // Enregistrez le classeur
            workbook.Save("FindMethodDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Find(object, Cell, FindOptions) {#find_1}

Trouve la cellule contenant l'objet d'entrée.

```csharp
public Cell Find(object what, Cell previousCell, FindOptions findOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| quoi | Object | L'objet à rechercher. Le type doit être int,double,DateTime,string,bool. |
| previousCell | Cellule | Cellule précédente avec le même objet. Ce paramètre peut être défini sur null si la recherche commence depuis le début. |
| findOptions | FindOptions | Options de recherche |

### Valeur de retour

Objet Cell.

### Remarques

Renvoie null (Nothing) si aucune cellule n'est trouvée.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodFindWithObjectCellFindOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir des données d'exemple
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["A2"].PutValue("def");
            worksheet.Cells["A3"].PutValue("abc ");
            
            // Créer des options de recherche
            FindOptions options = new FindOptions();
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;
            
            // Trouver la cellule avec la valeur "abc "
            Cell foundCell = worksheet.Cells.Find("abc ", null, options);
            
            Console.WriteLine("Found cell: " + (foundCell != null ? foundCell.Name : "null"));
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [FindOptions](../../findoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


