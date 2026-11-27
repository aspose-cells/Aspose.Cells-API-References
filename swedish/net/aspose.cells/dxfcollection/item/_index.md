---
title: "DxfCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DxfCollection-egenskap. Hämtar elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells/dxfcollection/item/
---
## DxfCollection indexer

Hämtar elementet på det angivna indexet.

```csharp
public Style this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det angivna indexet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DxfCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till DxfCollection från arbetsboken
            DxfCollection dxfCollection = workbook.Worksheets.Dxfs;

            // Skapa en ny stil (kan inte läggas till direkt i DxfCollection eftersom den saknar Add-metod)
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            // Stil läggs automatiskt till i samlingen när den skapas

            // Hämta det första objektet från DxfCollection med Item-egenskapen
            Style firstStyle = dxfCollection[0];
            Console.WriteLine("First style font name: " + firstStyle.Font.Name);

            // Modifiera stilen via Item-egenskapen (eftersom den returnerar en referens)
            firstStyle.Font.Color = System.Drawing.Color.Red;
            firstStyle.Font.IsBold = true;

            // Verifiera ändringen
            Console.WriteLine("Modified style font color: " + dxfCollection[0].Font.Color);
            Console.WriteLine("Modified style font bold: " + dxfCollection[0].Font.IsBold);

            // Applicera stilen på en cell för att se effekten
            worksheet.Cells["A1"].PutValue("DxfCollection Property Item Demo");
            worksheet.Cells["A1"].SetStyle(dxfCollection[0]);

            // Spara resultatet
            workbook.Save("DxfCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [DxfCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


