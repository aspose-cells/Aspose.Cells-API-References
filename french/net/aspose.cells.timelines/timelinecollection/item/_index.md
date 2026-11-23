---
title: "TimelineCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TimelineCollection. Obtient la Timeline par indice"
type: docs
url: /fr/net/aspose.cells.timelines/timelinecollection/item/
---
## TimelineCollection indexer (1 of 2)

Obtient la Timeline par indice.

```csharp
public Timeline this[int index] { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Timelines;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(DateTime.Now);
            sheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            
            // Créer d'abord le tableau croisé dynamique
            int pivotIndex = sheet.PivotTables.Add("A1:A3", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Ajouter la timeline à la feuille de calcul
            int index = sheet.Timelines.Add(pivotTable, 0, 0, "Date");
            
            // Accéder à la timeline en utilisant la propriété Item par indice
            Timeline timelineByIndex = sheet.Timelines[index];
            
            // Démontrer l'utilisation de la timeline
            Console.WriteLine("Timeline name: " + timelineByIndex.Name);
        }
    }
}
```

### Voir aussi

* class [Timeline](../../timeline/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## TimelineCollection indexer (2 of 2)

Obtient la Timeline par le nom de la Timeline.

```csharp
public Timeline this[string name] { get; }
```

### Exemples

```csharp

[C#]

//Obtenir la Timeline par le nom de la Timeline.
Timeline objByName = sheet.Timelines["date"];
```

### Voir aussi

* class [Timeline](../../timeline/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


