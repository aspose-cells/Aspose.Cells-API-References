---
title: "ActiveXControlBase.Workbook"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ActiveXControlBase-Eigenschaft. Gibt das Workbook-Objekt zurück"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/
---
## ActiveXControlBase.Workbook property

Gibt das `Workbook`-Objekt zurück.

```csharp
public Workbook Workbook { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Fügen Sie ein ActiveX-Steuerelement zum Arbeitsblatt hinzu
                Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 1, 0, 100, 30);
                CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

                // Setzen Sie einige Eigenschaften, um das Beispiel sinnvoll zu machen
                checkBox.Caption = "Sample CheckBox";
                checkBox.IsAutoSize = true;

                // Demonstrieren Sie die Workbook-Eigenschaft (schreibgeschützt)
                Workbook controlWorkbook = checkBox.Workbook;
                Console.WriteLine("ActiveX Control Workbook reference obtained successfully.");
                Console.WriteLine("Workbook has " + controlWorkbook.Worksheets.Count + " worksheets.");

                // Überprüfen Sie, ob die Workbook-Referenz dieselbe ist wie unser ursprüngliches Workbook
                if (controlWorkbook == workbook)
                {
                    Console.WriteLine("The ActiveX control's Workbook property correctly references the parent workbook.");
                }

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [Workbook](../../../aspose.cells/workbook/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


