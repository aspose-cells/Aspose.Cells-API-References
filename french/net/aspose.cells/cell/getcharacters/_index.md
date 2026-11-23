---
title: "Cell.GetCharacters"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Retourne tous les objets Characters qui représentent une plage de caractères dans le texte de la cellule"
type: docs
url: /fr/net/aspose.cells/cell/getcharacters/
---
## GetCharacters() {#getcharacters}

Renvoie tous les objets Characters qui représentent une plage de caractères dans le texte de la cellule.

```csharp
public FontSetting[] GetCharacters()
```

### Valeur de retour

Tous les objets Characters

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetCharactersDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir du texte formaté en HTML dans la cellule A1 avec différentes parties de mise en forme
            worksheet.Cells["A1"].HtmlString = "Normal text<div style=\"color: red;\">Red text</div>";

            // Obtenir les informations de mise en forme des caractères depuis la cellule A1
            FontSetting[] fontSettings = worksheet.Cells["A1"].GetCharacters();

            // Afficher les informations de mise en forme
            Console.WriteLine("Character formatting in cell A1:");
            for (int i = 0; i < fontSettings.Length; i++)
            {
                Console.WriteLine($"Part {i + 1}:");
                Console.WriteLine($"Start index: {fontSettings[i].StartIndex}");
                Console.WriteLine($"Length: {fontSettings[i].Length}");
                Console.WriteLine($"Font color: {fontSettings[i].Font.Color}");
                Console.WriteLine();
            }
        }
    }
}
```

### Voir aussi

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCharacters(bool) {#getcharacters_1}

Renvoie tous les objets Characters qui représentent une plage de caractères dans le texte de la cellule.

```csharp
public FontSetting[] GetCharacters(bool flag)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| flag | Boolean | Indique si le style de tableau est appliqué à la cellule lorsque la cellule se trouve dans le tableau. |

### Valeur de retour

Tous les objets Characters

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodGetCharactersWithBooleanDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter du texte à la cellule C8 avec mise en forme
            Cell cell = worksheet.Cells["C8"];
            cell.PutValue("Formatted Text");
            
            // Formater des portions du texte
            FontSetting fs1 = cell.Characters(0, 8);
            fs1.Font.Color = System.Drawing.Color.White;
            
            FontSetting fs2 = cell.Characters(9, 4);
            fs2.Font.Color = System.Drawing.Color.Blue;
            
            // Obtenir tous les paramètres de police avec le formatage
            FontSetting[] fontSettings = cell.GetCharacters(true);
            
            // Afficher les couleurs de police
            Console.WriteLine("Font colors in cell C8:");
            foreach (FontSetting fs in fontSettings)
            {
                Console.WriteLine(fs.Font.Color);
            }
        }
    }
}
```

### Voir aussi

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


