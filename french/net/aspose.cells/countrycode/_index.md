---
title: "Énumération CountryCode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.CountryCode. Représente les identifiants de pays Excel"
type: docs
url: /fr/net/aspose.cells/countrycode/
---
## CountryCode enumeration

Représente les identifiants de pays Excel.

```csharp
public enum CountryCode
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Default | `0` |  |
| USA | `1` | États-Unis |
| Canada | `2` | Canada |
| LatinAmeric | `3` | Amérique latine, sauf le Brésil |
| Russia | `7` | Russie |
| Egypt | `20` | Égypte |
| Greece | `30` | Grèce |
| Netherlands | `31` | Pays-Bas |
| Belgium | `32` | Belgique |
| France | `33` | France |
| Spain | `34` | Espagne |
| Hungary | `36` | Hongrie |
| Italy | `39` | Italie |
| Switzerland | `41` | Suisse |
| Austria | `43` | Autriche |
| UnitedKingdom | `44` | Royaume-Uni |
| Denmark | `45` | Danemark |
| Sweden | `46` | Suède |
| Norway | `47` | Norvège |
| Poland | `48` | Pologne |
| Germany | `49` | Allemagne |
| Mexico | `52` | Mexique |
| Brazil | `55` | Brésil |
| Australia | `61` | Australie |
| NewZealand | `64` | Nouvelle-Zélande |
| Thailand | `66` | Thaïlande |
| Japan | `81` | Japon |
| SouthKorea | `82` | Corée du Sud |
| VietNam | `84` | Viêt Nam |
| China | `86` | République populaire de Chine |
| Turkey | `90` | Turquie |
| India | `91` | Inde |
| Algeria | `213` | Algérie |
| Morocco | `216` | Maroc |
| Libya | `218` | Libye |
| Portugal | `351` | Portugal |
| Iceland | `354` | Islande |
| Finland | `358` | Finlande |
| Czech | `420` | République tchèque |
| Taiwan | `886` | Taïwan |
| Lebanon | `961` | Liban |
| Jordan | `962` | Jordanie |
| Syria | `963` | Syrie |
| Iraq | `964` | Irak |
| Kuwait | `965` | Koweït |
| Saudi | `966` | Arabie Saoudite |
| UnitedArabEmirates | `971` | Émirats arabes unis |
| Israel | `972` | Israël |
| Qatar | `974` | Qatar |
| Iran | `981` | Iran |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CountryCodeDemo
    {
        public static void CountryCodeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir le code pays pour le classeur
            workbook.Settings.LanguageCode = CountryCode.USA;
            workbook.Settings.Region = CountryCode.USA;

            // Ajouter des données à la feuille de calcul
            worksheet.Cells[0, 0].PutValue("Country");
            worksheet.Cells[0, 1].PutValue("Code");

            worksheet.Cells[1, 0].PutValue("United States");
            worksheet.Cells[1, 1].PutValue((int)CountryCode.USA);

            worksheet.Cells[2, 0].PutValue("Canada");
            worksheet.Cells[2, 1].PutValue((int)CountryCode.Canada);

            worksheet.Cells[3, 0].PutValue("France");
            worksheet.Cells[3, 1].PutValue((int)CountryCode.France);

            worksheet.Cells[4, 0].PutValue("Germany");
            worksheet.Cells[4, 1].PutValue((int)CountryCode.Germany);

            // Enregistrez le classeur
            workbook.Save("CountryCodeExample.xlsx");
            workbook.Save("CountryCodeExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


