---
title: "Style.ParentStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Hämtar förälderstilen för denna stil"
type: docs
url: /sv/net/aspose.cells/style/parentstyle/
---
## Style.ParentStyle property

Hämtar den överordnade stilen för denna stil.

```csharp
public Style ParentStyle { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StylePropertyParentStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Hämta det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].Value = "Parent Style Example";
            worksheet.Cells["A2"].Value = "Child Style Example";

            try
            {
                // Skapa en förälderstil
                Style parentStyle = workbook.CreateStyle();
                parentStyle.Font.Name = "Arial";
                parentStyle.Font.Size = 12;
                parentStyle.ForegroundColor = System.Drawing.Color.LightBlue;
                parentStyle.Pattern = BackgroundType.Solid;

                // Skapa en understil baserad på förälderstilen
                Style childStyle = workbook.CreateStyle();
                childStyle.Font.IsBold = true;
                childStyle.Font.Color = System.Drawing.Color.Red;

                // Tillämpa stilar på celler
                Cell parentCell = worksheet.Cells["A1"];
                parentCell.SetStyle(parentStyle);

                Cell childCell = worksheet.Cells["A2"];
                childCell.SetStyle(childStyle);

                // Demonstrera ParentStyle-egenskapen (skrivskyddad)
                Style retrievedChildStyle = childCell.GetStyle();
                Console.WriteLine("Child style has parent style: " +
                    (retrievedChildStyle.ParentStyle != null));

                if (retrievedChildStyle.ParentStyle != null)
                {
                    Console.WriteLine("Parent style font name: " +
                        retrievedChildStyle.ParentStyle.Font.Name);
                    Console.WriteLine("Parent style font size: " +
                        retrievedChildStyle.ParentStyle.Font.Size);
                }

                // Spara arbetsboken
                workbook.Save("ParentStyleDemo.xlsx");
                Console.WriteLine("ParentStyle demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


