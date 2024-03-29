---
title: RemoveDateFilter
second_title: Référence de l'API Aspose.Cells pour .NET
description: Supprime un filtre de date.
type: docs
weight: 180
url: /fr/net/aspose.cells/autofilter/removedatefilter/
---
## AutoFilter.RemoveDateFilter method

Supprime un filtre de date.

```csharp
public void RemoveDateFilter(int fieldIndex, DateTimeGroupingType dateTimeGroupingType, int year, 
    int month, int day, int hour, int minute, int second)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| fieldIndex | Int32 | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |
| dateTimeGroupingType | DateTimeGroupingType | [`DateTimeGroupingType`](../../datetimegroupingtype) |
| year | Int32 | L'année. |
| month | Int32 | Le mois. |
| day | Int32 | Le jour. |
| hour | Int32 | L'heure. |
| minute | Int32 | La minute. |
| second | Int32 | La deuxième. |

### Remarques

Si DateTimeGroupingType est Year, seuls les effets de l'année param. Si DateTiemGroupingType est Month, seuls les effets de l'année et du mois param.

### Voir également

* enum [DateTimeGroupingType](../../datetimegroupingtype)
* class [AutoFilter](../../autofilter)
* espace de noms [Aspose.Cells](../../autofilter)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
