---
title: remove_date_filter méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 150
url: /fr/python-net/aspose.cells/autofilter/remove_date_filter/
is_root: false
---
##  remove_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second) {#int-DateTimeGroupingType-int-int-int-int-int-int}
Supprime un filtre de date.



```python
def remove_date_filter(self, field_index, date_time_grouping_type, year, month, day, hour, minute, second):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| field_index | int | Le décalage entier du champ sur lequel vous souhaitez baser le filtre<br/> (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0).|
| date_time_grouping_type | [DateTimeGroupingType](/cells/fr/python-net/aspose.cells/datetimegroupingtype) | [DateTimeGroupingType](/cells/fr/python-net/aspose.cells/datetimegroupingtype) |
| year | int | L'année.|
| month | int | Le mois.|
| day | int | Le jour.|
| hour | int | L'heure.|
| minute | int | La minute.|
| second | int | La deuxième.|
###  Remarques

Si DateTimeGroupingType est Year, seul le paramètre year a un effet.
Si DateTiemGroupingType est Mois, seuls les paramètres année et mois ont un effet.


###  Voir également
* module [aspose.cells](../../)
* classe [AutoFilter](/cells/fr/python-net/aspose.cells/autofilter)
* classe [DateTimeGroupingType](/cells/fr/python-net/aspose.cells/datetimegroupingtype)
