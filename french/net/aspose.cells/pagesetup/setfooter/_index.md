---
title: "PageSetup.SetFooter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PageSetup. Définit un script formatant le pied de page d'un fichier Excel"
type: docs
url: /fr/net/aspose.cells/pagesetup/setfooter/
---
## PageSetup.SetFooter method

Définit un script formatant le pied de page d'un fichier Excel.

```csharp
public void SetFooter(int section, string footerScript)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| section | Int32 | 0 : Section gauche, 1 : Section centrale, 2 : Section droite. |
| footerScript | String | Script de format du pied de page. |

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

Par exemple : "&amp;Arial,Bold&amp;8Footer Note"

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFooterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.PageSetup.SetFooter(0, "Page &P");
            worksheet.PageSetup.SetFooter(1, "&D");
            worksheet.PageSetup.SetFooter(2, "&A");
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


