---
title: "Enum AccessCacheOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.AccessCacheOptions enum. Options de mise en cache pour l'accès aux données. Plusieurs options peuvent être combinées en utilisant l'opérateur  "
type: docs
url: /fr/net/aspose.cells/accesscacheoptions/
---
## AccessCacheOptions enumeration

Options de mise en cache pour l'accès aux données. Plusieurs options peuvent être combinées en utilisant l'opérateur "&#x7C;".

```csharp
[Flags]
public enum AccessCacheOptions
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Pas de cache pour aucun accès aux données. |
| All | `FFFFFFFFFFFFFFFF` | Appliquez toutes les optimisations possibles pour tous les types d'accès aux données dans le classeur. Tous les paramètres et données ne doivent pas être modifiés pendant l'accès optimisé. |
| PositionAndSize | `3` | Appliquer une optimisation possible pour obtenir la position et la taille de l'objet (tel que Shape). Les paramètres de hauteur de ligne et de largeur de colonne ne doivent pas être modifiés pendant l'accès optimisé. |
| CellsData | `9` | Appliquer une optimisation possible pour obtenir les valeurs des cellules. Les données des cellules (données et paramètres de Cell, Row) ne doivent pas être modifiées pendant l'accès optimisé, aucun nouvel objet Cell/Row ne doit être créé non plus (tel que par [`Item`](../cells/item/)). |
| CellDisplay | `100086` | Appliquer une optimisation possible pour obtenir les résultats liés à l'affichage des cellules ([`DisplayStringValue`](../cell/displaystringvalue/), [`GetStyle`](../cell/getstyle/), [`GetDisplayStyle`](../cell/getdisplaystyle/), etc.). Les données des cellules et les objets liés au style (styles Cell/Row/Column, largeur de colonne, etc.) ne doivent pas être modifiés pendant l'accès optimisé. |
| GetFormula | `200000` | Appliquer une optimisation possible pour obtenir les formules. Toutes les données et paramètres pouvant affecter l'expression de la formule (nom de la feuille de calcul, texte du nom, colonne du tableau, etc.) ne doivent pas être modifiés pendant l'accès optimisé. |
| SetFormula | `400000` | Appliquer une optimisation possible pour définir les formules. Toutes les données et paramètres pouvant affecter l'expression de la formule (nom de la feuille de calcul, texte du nom, colonne du tableau, etc.) ne doivent pas être modifiés pendant l'accès optimisé. |
| CalculateFormula | `800009` | Appliquer une optimisation possible pour calculer les formules. Les données des cellules ne doivent pas être modifiées pendant l'accès optimisé, aucun nouvel objet (Cell, Row, etc.) ne doit être créé non plus (tel que par [`Item`](../cells/item/)). |
| ConditionalFormatting | `1000009` | Appliquer une optimisation possible pour obtenir le résultat du formatage conditionnel. Toutes les données et paramètres pouvant affecter le résultat du formatage conditionnel (paramètres du formatage conditionnel, valeurs des cellules dépendantes, etc.) ne doivent pas être modifiés pendant l'accès optimisé. |
| Validation | `2000009` | Appliquer une optimisation possible pour obtenir le résultat de la validation. Toutes les données et paramètres pouvant affecter le résultat de la validation (paramètres de la validation, valeurs des cellules dépendantes, etc.) ne doivent pas être modifiés pendant l'accès optimisé. |

### Remarques

Pour certaines fonctionnalités, l'accès à un grand ensemble de données nécessite de nombreuses opérations répétées et complexes telles que la recherche, le calcul, ...etc., et ces opérations prendront beaucoup de temps supplémentaire. Dans les situations courantes, toutes les données dépendantes restent inchangées pendant l'accès, de sorte que des caches peuvent être créés et utilisés pour améliorer les performances d'accès. À cette fin, nous fournissons cette API afin que l'utilisateur puisse spécifier quel type d'accès aux données doit être optimisé par un mécanisme de mise en cache éventuel. Veuillez noter que, selon les options, différents ensembles de données peuvent devoir être en lecture seule ("read-only"). Et les performances d'accès aux données dépendent de nombreux aspects ; l'utilisation du mécanisme de mise en cache ne garantit pas une amélioration des performances. Dans certaines situations, comme lorsque l'ensemble de données à accéder est petit, l'utilisation du cache peut même prendre plus de temps, car la mise en cache elle‑même nécessite également un certain temps supplémentaire.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AccessCacheOptionsDemo
    {
        public static void AccessCacheOptionsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Démarrer le cache d'accès avec des options spécifiques
            workbook.StartAccessCache(AccessCacheOptions.PositionAndSize | AccessCacheOptions.CellsData);

            // Effectuer certaines opérations qui bénéficient de la mise en cache
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue(i + j);
                }
            }

            // Fermer le cache d'accès
            workbook.CloseAccessCache(AccessCacheOptions.PositionAndSize | AccessCacheOptions.CellsData);

            // Enregistrez le classeur
            workbook.Save("AccessCacheOptionsExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


