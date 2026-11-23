---
title: "DataSorter.AddColorKey"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode DataSorter. Ajoute une clé de tri de couleur"
type: docs
url: /fr/net/aspose.cells/datasorter/addcolorkey/
---
## DataSorter.AddColorKey method

Ajoute une clé de tri de couleur.

```csharp
public void AddColorKey(int key, SortOnType type, SortOrder order, Color color)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| clé | Int32 | L'index de la colonne triée (position absolue, la colonne A est 0, B est 1, ...) |
| type | SortOnType | Le type de valeur de couleur triée. |
| ordre | SortOrder | L'ordre de tri. |
| color | Color | La couleur de tri personnalisée. |

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddColorKeyWithInt32SortOnTypeSortOrderColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple avec des cellules colorées
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue(5);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(7);
            
            // Appliquez des couleurs aux cellules
            Style styleRed = workbook.CreateStyle();
            styleRed.ForegroundColor = Color.Red;
            styleRed.Pattern = BackgroundType.Solid;
            worksheet.Cells["A2"].SetStyle(styleRed);
            
            Style styleBlue = workbook.CreateStyle();
            styleBlue.ForegroundColor = Color.Blue;
            styleBlue.Pattern = BackgroundType.Solid;
            worksheet.Cells["A3"].SetStyle(styleBlue);
            
            Style styleGreen = workbook.CreateStyle();
            styleGreen.ForegroundColor = Color.Green;
            styleGreen.Pattern = BackgroundType.Solid;
            worksheet.Cells["A4"].SetStyle(styleGreen);

            // Créer un trieur de données et ajouter la clé de couleur
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;
            sorter.AddColorKey(0, SortOnType.CellColor, SortOrder.Ascending, Color.Red);

            // Trier les données
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A4"));

            // Afficher les valeurs triées (à titre de démonstration)
            Console.WriteLine("Sorted values:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + (i + 1)].IntValue);
            }
        }
    }
}
```

### Voir aussi

* enum [SortOnType](../../sortontype/)
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


