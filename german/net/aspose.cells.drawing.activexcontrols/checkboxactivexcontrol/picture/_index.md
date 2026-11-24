---
title: "CheckBoxActiveXControl.Picture"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CheckBoxActiveXControl-Eigenschaft. Ruft die Daten des Bildes ab und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/picture/
---
## CheckBoxActiveXControl.Picture property

Liest und setzt die Bilddaten.

```csharp
public byte[] Picture { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // CheckBox ActiveX-Steuerelement hinzufügen
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 2, 0, 2, 0, 100, 30);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Grundlegende Eigenschaften konfigurieren
            checkBox.Caption = "Custom CheckBox";
            checkBox.GroupName = "Group1";
            checkBox.Value = CheckValueType.UnChecked; // Fixed enum value casing

            // Anfangszustand des Bildes anzeigen
            Console.WriteLine("Initial Picture bytes: " + (checkBox.Picture == null ? "null" : checkBox.Picture.Length + " bytes"));

            try
            {
                // Bilddatei laden
                byte[] imageBytes = File.ReadAllBytes("checkbox_image.png");
                
                // Steuerungsbild und Position festlegen
                checkBox.Picture = imageBytes;
                checkBox.PicturePosition = ControlPicturePositionType.LeftTop;

                Console.WriteLine("Picture set successfully - " + checkBox.Picture.Length + " bytes");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error setting picture: " + ex.Message);
            }

            // Modifizierte Arbeitsmappe speichern
            workbook.Save("CheckBoxWithPicture.xlsx");
        }
    }
}
```

### Siehe auch

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


