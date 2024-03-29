---
title: Add
second_title: Référence de l'API Aspose.Cells pour .NET
description: Ajoute une feuille de calcul à la collection.
type: docs
weight: 170
url: /fr/net/aspose.cells/worksheetcollection/add/
---
## Add(SheetType) {#add_2}

Ajoute une feuille de calcul à la collection.

```csharp
public int Add(SheetType type)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| type | SheetType | Type de feuille de calcul. |

### Return_Value

[`Worksheet`](../../worksheet) indice d'objet.

### Exemples

```csharp
[C#]
Workbook workbook = new Workbook();
workbook.Worksheets.Add(SheetType.Chart);
Cells cells = workbook.Worksheets[0].Cells;
cells["c2"].PutValue(5000);
cells["c3"].PutValue(3000);
cells["c4"].PutValue(4000);
cells["c5"].PutValue(5000);
cells["c6"].PutValue(6000);
ChartCollection charts = workbook.Worksheets[1].Charts;
int chartIndex = charts.Add(ChartType.Column, 10,10,20,20);
Chart chart = charts[chartIndex];
chart.NSeries.Add("Sheet1!C2:C6", true);

[Visual Basic]
Dim workbook As Workbook =  New Workbook() 
workbook.Worksheets.Add(SheetType.Chart)
Dim cells As Cells = workbook.Worksheets(0).Cells 
cells("c2").PutValue(5000)
cells("c3").PutValue(3000)
cells("c4").PutValue(4000)
cells("c5").PutValue(5000)
cells("c6").PutValue(6000)
Dim charts As ChartCollection = workbook.Worksheets(1).Charts
Dim chartIndex As Integer = charts.Add(ChartType.Column,10,10,20,20) 
Dim chart As Chart = charts(chartIndex) 
chart.NSeries.Add("Sheet1!C2:C6", True)
```

### Voir également

* enum [SheetType](../../sheettype)
* class [WorksheetCollection](../../worksheetcollection)
* espace de noms [Aspose.Cells](../../worksheetcollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add() {#add_1}

Ajoute une feuille de calcul à la collection.

```csharp
public int Add()
```

### Return_Value

[`Worksheet`](../../worksheet) indice d'objet.

### Voir également

* class [WorksheetCollection](../../worksheetcollection)
* espace de noms [Aspose.Cells](../../worksheetcollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(string) {#add}

Ajoute une feuille de calcul à la collection.

```csharp
public Worksheet Add(string sheetName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| sheetName | String | Nom de la feuille de calcul |

### Return_Value

[`Worksheet`](../../worksheet) objet.

### Voir également

* class [Worksheet](../../worksheet)
* class [WorksheetCollection](../../worksheetcollection)
* espace de noms [Aspose.Cells](../../worksheetcollection)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
