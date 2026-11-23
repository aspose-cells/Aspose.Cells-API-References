---
title: "PageSetup.SetHeader"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PageSetup. Définit un script formatant l’en-tête d’un fichier Excel"
type: docs
url: /fr/net/aspose.cells/pagesetup/setheader/
---
## PageSetup.SetHeader method

Définit un script formatant l'en-tête d'un fichier Excel.

```csharp
public void SetHeader(int section, string headerScript)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| section | Int32 | 0 : Section gauche, 1 : Section centrale, 2 : Section droite. |
| headerScript | String | Script de format d’en-tête. |

### Remarques

Commandes du script :

| **Command** | **Description** |
| --- | --- |
| &amp;P | Numéro de page actuel |
| &amp;N | Nombre de pages |
| &amp;D | Date actuelle |
| &amp;T | Heure actuelle |
| &amp;A | Nom de la feuille |
| &amp;F | Nom de fichier sans le chemin |
| &amp;\"&lt;FontName&gt;\" | Nom de police, par exemple : &amp;\"Arial\" |
| &amp;\"&lt;FontName&gt;, &lt;FontStyle&gt;\" | Nom de police et style de police, par exemple : &amp;\"Arial,Bold\" |
| &amp;&lt;FontSize&gt; | Taille de police. Si cette commande est suivie d'un nombre simple à imprimer dans l'en-tête, il sera séparé de la hauteur de police par un caractère d'espace. |
| &amp;K&lt;RRGGBB&gt; | Couleur de police, par exemple (ROUGE) : &amp;KFF0000 |
| &amp;G | Script d'image |

Par exemple : "&amp;Arial,Bold&amp;8Header Note"

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Définir différentes sections d'en-tête avec diverses commandes
            pageSetup.SetHeader(0, "&F"); // Left section - File name
            pageSetup.SetHeader(1, "Page &P of &N"); // Center section - Page numbering
            pageSetup.SetHeader(2, "&D"); // Right section - Date

            workbook.Save("PageSetup_SetHeader_Example.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


