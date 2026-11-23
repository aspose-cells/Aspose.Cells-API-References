---
title: "WorksheetCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WorksheetCollection. Ajoute une feuille de calcul à la collection"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/add/
---
## Add(SheetType) {#add_2}

Ajoute une feuille de calcul à la collection.

```csharp
public int Add(SheetType type)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | SheetType | Type de feuille de calcul. |

### Valeur de retour

[`Worksheet`](../../worksheet/) object index.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddWithSheetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Ajouter une nouvelle feuille de graphique en utilisant le paramètre SheetType
            workbook.Worksheets.Add(SheetType.Chart);
            
            // Ajouter des données à la première feuille de calcul
            Cells cells = workbook.Worksheets[0].Cells;
            cells["C2"].PutValue(5000);
            cells["C3"].PutValue(3000);
            cells["C4"].PutValue(4000);
            cells["C5"].PutValue(5000);
            cells["C6"].PutValue(6000);
            
            // Créer un graphique dans la feuille de graphique
            Aspose.Cells.Charts.ChartCollection charts = workbook.Worksheets[1].Charts;
            int chartIndex = charts.Add(Aspose.Cells.Charts.ChartType.Column, 10, 10, 20, 20);
            Aspose.Cells.Charts.Chart chart = charts[chartIndex];
            chart.NSeries.Add("Sheet1!C2:C6", true);
            
            // Enregistrer le classeur (facultatif)
            // workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add() {#add_1}

Ajoute une feuille de calcul à la collection.

```csharp
public int Add()
```

### Valeur de retour

[`Worksheet`](../../worksheet/) object index.

### Voir aussi

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add}

Ajoute une feuille de calcul à la collection.

```csharp
public Worksheet Add(string sheetName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sheetName | String | Nom de la feuille de calcul |

### Valeur de retour

[`Worksheet`](../../worksheet/) object.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets.Add("NewSheet");
            
            // Ajouter des données à la nouvelle feuille de calcul
            worksheet.Cells["A1"].PutValue("Worksheet added successfully!");
            
            // Enregistrez le classeur
            wb.Save("WorksheetCollectionMethodAddWithStringDemo_output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


