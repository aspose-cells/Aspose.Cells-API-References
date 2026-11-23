---
title: "LoadOptions.Region"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LoadOptions. Obtient ou définit les paramètres régionaux utilisés pour le classeur qui sera chargé"
type: docs
url: /fr/net/aspose.cells/loadoptions/region/
---
## LoadOptions.Region property

Obtient ou définit les paramètres régionaux utilisés pour le classeur qui sera chargé.

```csharp
public CountryCode Region { get; set; }
```

### Remarques

Les paramètres régionaux peuvent être utilisés pour initialiser certaines fonctionnalités du classeur telles que les polices, les thèmes, etc. Pour les formats de fichiers basés sur du texte, comme CSV, HTML, ..., le paramètre régional sera également utilisé pour détecter les formats numériques et analyser les valeurs textuelles en valeurs numériques ou de date/heure pour les cellules. Ce paramètre sera conservé pour le classeur instancié ultérieurement, c’est‑à‑dire que le [`Region`](../../workbooksettings/region/) du classeur utilisera la même région que cette propriété.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyRegionDemo
    {
        public static void Run()
        {
            // Créer des options de chargement pour le fichier HTML
            LoadOptions loadOpts = new LoadOptions(LoadFormat.Html);
            
            // Définir la région sur USA
            loadOpts.Region = CountryCode.USA;
            
            // Charger le fichier HTML avec les paramètres régionaux spécifiés
            Workbook wb = new Workbook("example.html", loadOpts);
            
            // Accéder à la première feuille de calcul
            Worksheet ws = wb.Worksheets[0];
            
            // Démontrer le formatage spécifique à une région en vérifiant le style d'une cellule
            Style style = ws.Cells["A1"].GetStyle();
            Console.WriteLine("Font used in cell A1: " + style.Font.Name);
            Console.WriteLine("Region used for loading: " + loadOpts.Region);
        }
    }
}
```

### Voir aussi

* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


