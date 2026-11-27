---
title: "CheckBoxActiveXControl.Picture"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CheckBoxActiveXControl egenskap. Hämtar och anger data för bilden"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/picture/
---
## CheckBoxActiveXControl.Picture property

Hämtar och anger bildens data.

```csharp
public byte[] Picture { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;
    using System.IO;

    public class CheckBoxActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till CheckBox ActiveX‑kontroll
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 2, 0, 2, 0, 100, 30);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Konfigurera grundläggande egenskaper
            checkBox.Caption = "Custom CheckBox";
            checkBox.GroupName = "Group1";
            checkBox.Value = CheckValueType.UnChecked; // Fixed enum value casing

            // Visa initialt bildtillstånd
            Console.WriteLine("Initial Picture bytes: " + (checkBox.Picture == null ? "null" : checkBox.Picture.Length + " bytes"));

            try
            {
                // Läs in bildfil
                byte[] imageBytes = File.ReadAllBytes("checkbox_image.png");
                
                // Ställ in kontrollens bild och position
                checkBox.Picture = imageBytes;
                checkBox.PicturePosition = ControlPicturePositionType.LeftTop;

                Console.WriteLine("Picture set successfully - " + checkBox.Picture.Length + " bytes");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error setting picture: " + ex.Message);
            }

            // Spara modifierad arbetsbok
            workbook.Save("CheckBoxWithPicture.xlsx");
        }
    }
}
```

### Se även

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


