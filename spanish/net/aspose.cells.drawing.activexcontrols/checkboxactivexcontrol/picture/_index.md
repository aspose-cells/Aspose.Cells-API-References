---
title: "CheckBoxActiveXControl.Picture"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CheckBoxActiveXControl. Obtiene y establece los datos de la imagen"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/picture/
---
## CheckBoxActiveXControl.Picture property

Obtiene y establece los datos de la imagen.

```csharp
public byte[] Picture { get; set; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar control CheckBox ActiveX
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 2, 0, 2, 0, 100, 30);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Configurar propiedades básicas
            checkBox.Caption = "Custom CheckBox";
            checkBox.GroupName = "Group1";
            checkBox.Value = CheckValueType.UnChecked; // Fixed enum value casing

            // Mostrar el estado inicial de la Imagen
            Console.WriteLine("Initial Picture bytes: " + (checkBox.Picture == null ? "null" : checkBox.Picture.Length + " bytes"));

            try
            {
                // Cargar archivo de imagen
                byte[] imageBytes = File.ReadAllBytes("checkbox_image.png");
                
                // Establecer la imagen y la posición del control
                checkBox.Picture = imageBytes;
                checkBox.PicturePosition = ControlPicturePositionType.LeftTop;

                Console.WriteLine("Picture set successfully - " + checkBox.Picture.Length + " bytes");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error setting picture: " + ex.Message);
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("CheckBoxWithPicture.xlsx");
        }
    }
}
```

### Ver también

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


