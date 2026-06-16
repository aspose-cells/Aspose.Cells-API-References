---
title: Aspose::Cells::Drawing::Area::SetInvertIfNegative method
linktitle: SetInvertIfNegative
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Area::SetInvertIfNegative method. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged in C++.'
type: docs
weight: 1300
url: /fr/cpp/aspose.cells.drawing/area/setinvertifnegative/
---
## Area::SetInvertIfNegative method


If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```cpp
void Aspose::Cells::Drawing::Area::SetInvertIfNegative(bool value)
```


## Examples


```cpp
Aspose::Cells::Startup();
//Instanciation d'un objet Workbook
Workbook workbook;
//Ajout d'une nouvelle feuille de calcul à l'objet Workbook
int sheetIndex = workbook.GetWorksheets().Add();
//Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son index de feuille
Worksheet worksheet = workbook.GetWorksheets().Get(sheetIndex);
//Ajouter une valeur d'exemple à la cellule \"A1\"
worksheet.GetCells().Get(u"A1").PutValue(50);
//Ajouter une valeur d'exemple à la cellule \"A2\"
worksheet.GetCells().Get(u"A2").PutValue(-100);
//Ajouter une valeur d'exemple à la cellule \"A3\"
worksheet.GetCells().Get(u"A3").PutValue(150);
//Ajouter un graphique à la feuille de calcul
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//Accéder à l'instance du graphique nouvellement ajouté
Chart chart = worksheet.GetCharts().Get(chartIndex);
//Ajout de NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "A3"
chart.GetNSeries().Add(u"A1:A3", true);
chart.GetNSeries().Get(0).GetArea().SetInvertIfNegative(true);
//Définir la couleur de premier plan de la zone du 1er NSeries
chart.GetNSeries().Get(0).GetArea().SetForegroundColor(Color{ 0xff, 0xff, 0, 0 });
//Définir la couleur d'arrière-plan de la première zone NSeries.
//La couleur de zone affichée du deuxième point du graphique sera la couleur d'arrière-plan.
chart.GetNSeries().Get(0).GetArea().SetBackgroundColor(Color{ 0xff, 0xff, 0xff, 0 });
//Enregistrement du fichier Excel
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Class [Area](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
