---
title: "Enumération SmartTagShowType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enumération Aspose.Cells.Markup.SmartTagShowType. Représente le type d'affichage du smart tag"
type: docs
url: /fr/net/aspose.cells.markup/smarttagshowtype/
---
## SmartTagShowType enumeration

Représente le type d'affichage de la balise intelligente.

```csharp
public enum SmartTagShowType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| All | `0` | Indique que les smart tags sont activés et affichés |
| NoSmartTagIndicator | `1` | Indique que les smart tags sont activés mais que l'indicateur n'est pas affiché. |
| None | `2` | Indique que les smart tags sont désactivés et ne sont pas affichés. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagShowTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Démontre toutes les valeurs de l'énumération SmartTagShowType
            Console.WriteLine("SmartTagShowType values:");
            Console.WriteLine($"All: {SmartTagShowType.All}");
            Console.WriteLine($"NoSmartTagIndicator: {SmartTagShowType.NoSmartTagIndicator}");
            Console.WriteLine($"None: {SmartTagShowType.None}");

            // Crée et configure un smart tag
            var smartTagCollection = worksheet.SmartTagSetting.Add("urn:schemas-microsoft-com:office:smarttags#date");

            // Définit les propriétés qui utiliseraient SmartTagShowType (simulé car la propriété réelle n'est pas disponible)
            Console.WriteLine("\nSmart tag created at A1 with current date");

            // Enregistre avec différents scénarios de type d'affichage
            workbook.Save("SmartTagShowTypeDemo_All.xlsx");
            Console.WriteLine("Workbook saved with default show type (All)");

            // Crée un autre classeur avec un comportement de type d'affichage différent
            Workbook workbook2 = new Workbook();
            Worksheet worksheet2 = workbook2.Worksheets[0];
            worksheet2.SmartTagSetting.Add("urn:schemas-microsoft-com:office:smarttags#date");
            Console.WriteLine("\nSecond workbook created with smart tag at B2");

            workbook2.Save("SmartTagShowTypeDemo_None.xlsx");
            Console.WriteLine("Second workbook saved (simulating None behavior)");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


