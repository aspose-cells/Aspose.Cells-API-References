---
title: "CheckBoxActiveXControl.Picture"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CheckBoxActiveXControl. Ottiene e imposta i dati dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/picture/
---
## CheckBoxActiveXControl.Picture property

Ottiene e imposta i dati dell'immagine.

```csharp
public byte[] Picture { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi il controllo CheckBox ActiveX
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 2, 0, 2, 0, 100, 30);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Configura le proprietà di base
            checkBox.Caption = "Custom CheckBox";
            checkBox.GroupName = "Group1";
            checkBox.Value = CheckValueType.UnChecked; // Fixed enum value casing

            // Visualizza lo stato iniziale dell'immagine
            Console.WriteLine("Initial Picture bytes: " + (checkBox.Picture == null ? "null" : checkBox.Picture.Length + " bytes"));

            try
            {
                // Carica il file immagine
                byte[] imageBytes = File.ReadAllBytes("checkbox_image.png");
                
                // Imposta l'immagine del controllo e la posizione
                checkBox.Picture = imageBytes;
                checkBox.PicturePosition = ControlPicturePositionType.LeftTop;

                Console.WriteLine("Picture set successfully - " + checkBox.Picture.Length + " bytes");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error setting picture: " + ex.Message);
            }

            // Salvare la cartella di lavoro modificata
            workbook.Save("CheckBoxWithPicture.xlsx");
        }
    }
}
```

### Vedi anche

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


