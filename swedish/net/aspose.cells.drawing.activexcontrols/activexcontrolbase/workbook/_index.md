---
title: "ActiveXControlBase.Workbook"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ActiveXControlBase-egenskap. Hämtar Workbook‑objektet"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/
---
## ActiveXControlBase.Workbook property

Hämtar `Workbook`‑objektet.

```csharp
public Workbook Workbook { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlBasePropertyWorkbookDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till en ActiveX-kontroll på kalkylbladet
                Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 1, 0, 100, 30);
                CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

                // Ställ in några egenskaper för att göra exemplet meningsfullt
                checkBox.Caption = "Sample CheckBox";
                checkBox.IsAutoSize = true;

                // Visa Workbook‑egenskapen (skrivskyddad)
                Workbook controlWorkbook = checkBox.Workbook;
                Console.WriteLine("ActiveX Control Workbook reference obtained successfully.");
                Console.WriteLine("Workbook has " + controlWorkbook.Worksheets.Count + " worksheets.");

                // Verifiera att Workbook‑referensen är densamma som vår ursprungliga Workbook
                if (controlWorkbook == workbook)
                {
                    Console.WriteLine("The ActiveX control's Workbook property correctly references the parent workbook.");
                }

                // Spara arbetsboken
                workbook.Save("ActiveXControlWorkbookDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [Workbook](../../../aspose.cells/workbook/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


