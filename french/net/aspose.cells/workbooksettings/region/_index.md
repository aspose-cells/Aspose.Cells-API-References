---
title: "WorkbookSettings.Region"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient ou définit les paramètres régionaux du classeur"
type: docs
url: /fr/net/aspose.cells/workbooksettings/region/
---
## WorkbookSettings.Region property

Obtient ou définit les paramètres régionaux du classeur.

```csharp
public CountryCode Region { get; set; }
```

### Remarques

1. Paramètres régionaux utilisés par le composant Aspose.Cells pour un classeur chargé à partir d'un fichier modèle : i). Pour un fichier XLS, des champs sont définis pour les paramètres régionaux et MS Excel enregistre les données de paramètres régionaux dans le fichier lors de l'enregistrement du fichier XLS. Ainsi, nous utilisons la région enregistrée dans le fichier modèle pour le classeur. Si vous ne souhaitez pas utiliser la région enregistrée dans le fichier XLS, veuillez la réinitialiser à la valeur attendue (par exemple, CountryCode.Default) après le chargement du fichier modèle. De plus, nous enregistrons également la valeur spécifiée par l'utilisateur (via cette méthode) dans le fichier lors de l'enregistrement d'un fichier XLS. ii). Pour les autres formats de fichier, tels que XLSX, XLSB…etc., aucun champ n'est défini pour les paramètres régionaux dans la spécification du format de fichier. Ainsi, nous utilisons les paramètres régionaux de l'environnement de l'application pour le classeur. Et la valeur spécifiée par l'utilisateur (via cette méthode) ne peut pas être conservée pour les fichiers générés avec ces formats de fichier. 2. Pour l'effet d'affichage dans MS Excel : les paramètres régionaux appliqués ici ne peuvent prendre effet qu'à l'exécution avec le composant Aspose.Cells et non lors de la visualisation du fichier généré avec MS Excel. Même pour le fichier XLS généré dans lequel les données de paramètres régionaux spécifiées ont été enregistrées, lors de la visualisation/édition avec MS Excel, la région utilisée par MS Excel pour effectuer le formatage est toujours les paramètres régionaux par défaut de l'environnement où MS Excel s'exécute, et non celle enregistrée dans le fichier. C’est le comportement de MS Excel et il ne peut pas être modifié par le code.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRegionDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Japan;
            
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            cell.PutValue(44089); // Represents 2020-09-15
            
            Style style = cell.GetStyle();
            style.Custom = "[$-F800]yyyy年m月d日";
            cell.SetStyle(style);
            
            Console.WriteLine("Formatted value: " + cell.StringValue);
        }
    }
}
```

### Voir aussi

* enum [CountryCode](../../countrycode/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


