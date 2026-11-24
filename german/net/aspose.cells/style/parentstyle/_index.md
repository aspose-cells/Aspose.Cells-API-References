---
title: "Style.ParentStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt den übergeordneten Stil dieses Stils zurück"
type: docs
url: /de/net/aspose.cells/style/parentstyle/
---
## Style.ParentStyle property

Liest den übergeordneten Stil dieses Stils.

```csharp
public Style ParentStyle { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StylePropertyParentStyleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Hole das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "Parent Style Example";
            worksheet.Cells["A2"].Value = "Child Style Example";

            try
            {
                // Erstelle einen übergeordneten Stil
                Style parentStyle = workbook.CreateStyle();
                parentStyle.Font.Name = "Arial";
                parentStyle.Font.Size = 12;
                parentStyle.ForegroundColor = System.Drawing.Color.LightBlue;
                parentStyle.Pattern = BackgroundType.Solid;

                // Erstelle einen untergeordneten Stil basierend auf dem übergeordneten Stil
                Style childStyle = workbook.CreateStyle();
                childStyle.Font.IsBold = true;
                childStyle.Font.Color = System.Drawing.Color.Red;

                // Stile auf Zellen anwenden
                Cell parentCell = worksheet.Cells["A1"];
                parentCell.SetStyle(parentStyle);

                Cell childCell = worksheet.Cells["A2"];
                childCell.SetStyle(childStyle);

                // Demonstriere die ParentStyle-Eigenschaft (schreibgeschützt)
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

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


