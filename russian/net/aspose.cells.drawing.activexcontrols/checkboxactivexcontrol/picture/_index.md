---
title: "CheckBoxActiveXControl.Picture"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CheckBoxActiveXControl. Получает и задает данные изображения"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/picture/
---
## CheckBoxActiveXControl.Picture property

Получает и задает данные изображения.

```csharp
public byte[] Picture { get; set; }
```

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления CheckBox ActiveX
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 2, 0, 2, 0, 100, 30);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Настройте базовые свойства
            checkBox.Caption = "Custom CheckBox";
            checkBox.GroupName = "Group1";
            checkBox.Value = CheckValueType.UnChecked; // Fixed enum value casing

            // Отобразить начальное состояние изображения
            Console.WriteLine("Initial Picture bytes: " + (checkBox.Picture == null ? "null" : checkBox.Picture.Length + " bytes"));

            try
            {
                // Загрузить файл изображения
                byte[] imageBytes = File.ReadAllBytes("checkbox_image.png");
                
                // Установить изображение элемента управления и позицию
                checkBox.Picture = imageBytes;
                checkBox.PicturePosition = ControlPicturePositionType.LeftTop;

                Console.WriteLine("Picture set successfully - " + checkBox.Picture.Length + " bytes");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error setting picture: " + ex.Message);
            }

            // Сохранить изменённую книгу
            workbook.Save("CheckBoxWithPicture.xlsx");
        }
    }
}
```

### См. также

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


