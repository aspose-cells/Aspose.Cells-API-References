---
title: "OleObject.SetEmbeddedObject"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод OleObject. Устанавливает данные встроенного объекта"
type: docs
url: /ru/net/aspose.cells.drawing/oleobject/setembeddedobject/
---
## SetEmbeddedObject(bool, byte[], string, bool, string) {#setembeddedobject}

Задает данные вложенного объекта.

```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName, 
    bool displayAsIcon, string label)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| linkToFile | Boolean | Указывает, связывается ли объект с файлом. Если true, параметр objectData игнорируется. |
| objectData | Byte[] | Данные встроенного объекта. |
| sourceFileName | String | Имя файла. |
| displayAsIcon | Boolean | Указывает, отображать ли объект в виде значка. Если true, оригинальные данные изображения будут заменены значком. |
| label | String | Подпись значка. Работает только когда displayAsIcon равно true. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectMethodSetEmbeddedObjectWithBooleanByteArrayStringBooleanStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить OleObject в worksheet
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // Подготовьте параметры для SetEmbeddedObject
                bool linkToFile = false;
                byte[] objectData = File.ReadAllBytes("sample.xlsx");
                string sourceFileName = "sample.xlsx";
                bool displayAsIcon = false;
                string label = "Excel Document";

                // Вызовите SetEmbeddedObject с указанными параметрами
                oleObject.SetEmbeddedObject(linkToFile, objectData, sourceFileName, displayAsIcon, label);

                Console.WriteLine("SetEmbeddedObject executed successfully with parameters (Boolean, Byte[], String, Boolean, String)");
                
                // Отобразите некоторые свойства, чтобы показать эффект
                Console.WriteLine($"OleObject label: {oleObject.Label}");
                Console.WriteLine($"Display as icon: {oleObject.DisplayAsIcon}");
                Console.WriteLine($"Is linked to file: {oleObject.IsLink}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetEmbeddedObject method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("OleObjectMethodSetEmbeddedObjectDemo.xlsx");
        }
    }
}
```

### См. также

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## SetEmbeddedObject(bool, byte[], string, bool, string, bool) {#setembeddedobject_1}

Задает данные вложенного объекта.

```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName, 
    bool displayAsIcon, string label, bool updateIcon)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| linkToFile | Boolean | Указывает, связывается ли объект с файлом. Если true, параметр objectData игнорируется. |
| objectData | Byte[] | Данные встроенного объекта. |
| sourceFileName | String | Имя файла. |
| displayAsIcon | Boolean | Указывает, отображать ли объект в виде значка. Если true, оригинальные данные изображения будут заменены значком. |
| label | String | Подпись значка. Работает только когда displayAsIcon равно true. |
| updateIcon | Boolean | Указывает, обновлять ли значок автоматически. |

### Примечания

Поскольку Aspose может обновлять встроенные значки всех файлов, лучше добавить правильный значок, установив *updateIcon* в false.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectMethodSetEmbeddedObjectWithBooleanByteArrayStringBooleanStringBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить OleObject в worksheet
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // Подготовьте параметры для SetEmbeddedObject
                bool linkToFile = false;
                byte[] objectData = File.ReadAllBytes("sample.docx");
                string sourceFileName = "sample.docx";
                bool displayAsIcon = true;
                string label = "Word Document";
                bool updateIcon = true;

                // Вызовите SetEmbeddedObject с указанными параметрами
                oleObject.SetEmbeddedObject(linkToFile, objectData, sourceFileName, displayAsIcon, label, updateIcon);

                Console.WriteLine("SetEmbeddedObject executed successfully with parameters (Boolean, Byte[], String, Boolean, String, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetEmbeddedObject method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("OleObjectMethodSetEmbeddedObjectDemo.xlsx");
        }
    }
}
```

### См. также

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


