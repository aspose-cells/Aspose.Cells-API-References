---
title: "Style.ParentStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Ottiene lo stile genitore di questo stile"
type: docs
url: /it/net/aspose.cells/style/parentstyle/
---
## Style.ParentStyle property

Ottiene lo stile genitore di questo stile.

```csharp
public Style ParentStyle { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StylePropertyParentStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Ottieni il primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].Value = "Parent Style Example";
            worksheet.Cells["A2"].Value = "Child Style Example";

            try
            {
                // Crea uno stile genitore
                Style parentStyle = workbook.CreateStyle();
                parentStyle.Font.Name = "Arial";
                parentStyle.Font.Size = 12;
                parentStyle.ForegroundColor = System.Drawing.Color.LightBlue;
                parentStyle.Pattern = BackgroundType.Solid;

                // Crea uno stile figlio basato sullo stile genitore
                Style childStyle = workbook.CreateStyle();
                childStyle.Font.IsBold = true;
                childStyle.Font.Color = System.Drawing.Color.Red;

                // Applica gli stili alle celle
                Cell parentCell = worksheet.Cells["A1"];
                parentCell.SetStyle(parentStyle);

                Cell childCell = worksheet.Cells["A2"];
                childCell.SetStyle(childStyle);

                // Dimostra la proprietà ParentStyle (sola lettura)
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

                // Salva la cartella di lavoro
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

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


