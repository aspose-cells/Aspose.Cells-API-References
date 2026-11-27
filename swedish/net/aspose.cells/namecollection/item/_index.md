---
title: "NameCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "NameCollection-egenskapen. Hämtar Name-elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells/namecollection/item/
---
## NameCollection indexer (1 of 2)

Hämtar [`Name`](../../name/) elementet på det angivna indexet.

```csharp
public Name this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till några arbetsblad
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Åtkomst till namnsamlingen
            NameCollection names = workbook.Worksheets.Names;
            
            // Lägg till namngivna områden med korrekt metodsignatur
            int index1 = names.Add("Range1");
            names[index1].RefersTo = "=Sheet1!$A$1:$B$2";
            
            int index2 = names.Add("Range2");
            names[index2].RefersTo = "=Sheet2!$C$3:$D$4";
            
            int index3 = names.Add("Range3");
            names[index3].RefersTo = "=Sheet3!$E$5:$F$6";

            // Demonstrera användning av Item-egenskapen
            Console.WriteLine("Named Ranges:");
            for (int i = 0; i < names.Count; i++)
            {
                Name name = names[i]; // Using Item property with index
                Console.WriteLine($"{name.Text}: {name.RefersTo}");
            }

            // Åtkomst via namn med Item-egenskapen
            Name specificName = names["Range2"];
            Console.WriteLine($"\nSpecific Range: {specificName.Text} refers to {specificName.RefersTo}");

            // Ändra ett namngivet område
            names["Range3"].RefersTo = "=Sheet3!$A$1:$B$10";
            Console.WriteLine($"\nModified Range3 now refers to: {names["Range3"].RefersTo}");
        }
    }
}
```

### Se även

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## NameCollection indexer (2 of 2)

Hämtar [`Name`](../../name/) elementet med det angivna namnet.

```csharp
public Name this[string text] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| text | Namnetext. |

### Returvärde

Elementet med det angivna namnet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till arbetsbladens namnkollektion
            NameCollection names = workbook.Worksheets.Names;
            
            // Lägg till några namngivna områden (korrigerat för att använda korrekt Add‑metodsignatur)
            int index1 = names.Add("Range1");
            names[index1].RefersTo = "=Sheet1!$A$1:$A$10";
            
            int index2 = names.Add("Range2");
            names[index2].RefersTo = "=Sheet1!$B$1:$B$10";
            
            // Åtkomst till namngivna områden med Item‑egenskapen
            Name range1 = names["Range1"];
            Name range2 = names["Range2"];
            
            // Verifiera att namnen finns
            if (range1 != null && range2 != null)
            {
                Console.WriteLine("Named range 'Range1' refers to: " + range1.RefersTo);
                Console.WriteLine("Named range 'Range2' refers to: " + range2.RefersTo);
            }
            
            // Försök att komma åt ett icke‑existerande namn
            Name range3 = names["NonExistentRange"];
            if (range3 == null)
            {
                Console.WriteLine("Named range 'NonExistentRange' not found");
            }
        }
    }
}
```

### Se även

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


