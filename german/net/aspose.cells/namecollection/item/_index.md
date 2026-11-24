---
title: "NameCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "NameCollection-Eigenschaft. Gibt das Name-Element am angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells/namecollection/item/
---
## NameCollection indexer (1 of 2)

Gibt das [`Name`](../../name/) Element am angegebenen Index zurück.

```csharp
public Name this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der nullbasierte Index des Elements. |

### Rückgabewert

Das Element am angegebenen Index.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Einige Arbeitsblätter hinzufügen
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Greift auf die Namenssammlung zu
            NameCollection names = workbook.Worksheets.Names;
            
            // Fügen Sie benannte Bereiche mit der korrekten Methodensignatur hinzu
            int index1 = names.Add("Range1");
            names[index1].RefersTo = "=Sheet1!$A$1:$B$2";
            
            int index2 = names.Add("Range2");
            names[index2].RefersTo = "=Sheet2!$C$3:$D$4";
            
            int index3 = names.Add("Range3");
            names[index3].RefersTo = "=Sheet3!$E$5:$F$6";

            // Demonstriere die Verwendung der Item-Eigenschaft
            Console.WriteLine("Named Ranges:");
            for (int i = 0; i < names.Count; i++)
            {
                Name name = names[i]; // Using Item property with index
                Console.WriteLine($"{name.Text}: {name.RefersTo}");
            }

            // Zugriff per Name über die Item-Eigenschaft
            Name specificName = names["Range2"];
            Console.WriteLine($"\nSpecific Range: {specificName.Text} refers to {specificName.RefersTo}");

            // Ändern Sie einen benannten Bereich
            names["Range3"].RefersTo = "=Sheet3!$A$1:$B$10";
            Console.WriteLine($"\nModified Range3 now refers to: {names["Range3"].RefersTo}");
        }
    }
}
```

### Siehe auch

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## NameCollection indexer (2 of 2)

Gibt das [`Name`](../../name/) Element mit dem angegebenen Namen zurück.

```csharp
public Name this[string text] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Text | Name-Text. |

### Rückgabewert

Das Element mit dem angegebenen Namen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf die Namenssammlung der Arbeitsblätter zu
            NameCollection names = workbook.Worksheets.Names;
            
            // Fügen Sie einige benannte Bereiche hinzu (korrigiert, um die richtige Add-Methodensignatur zu verwenden)
            int index1 = names.Add("Range1");
            names[index1].RefersTo = "=Sheet1!$A$1:$A$10";
            
            int index2 = names.Add("Range2");
            names[index2].RefersTo = "=Sheet1!$B$1:$B$10";
            
            // Greifen Sie auf benannte Bereiche über die Item-Eigenschaft zu
            Name range1 = names["Range1"];
            Name range2 = names["Range2"];
            
            // Überprüfen Sie, ob die Namen existieren
            if (range1 != null && range2 != null)
            {
                Console.WriteLine("Named range 'Range1' refers to: " + range1.RefersTo);
                Console.WriteLine("Named range 'Range2' refers to: " + range2.RefersTo);
            }
            
            // Versuchen Sie, auf einen nicht existierenden Namen zuzugreifen
            Name range3 = names["NonExistentRange"];
            if (range3 == null)
            {
                Console.WriteLine("Named range 'NonExistentRange' not found");
            }
        }
    }
}
```

### Siehe auch

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


