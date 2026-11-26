---
title: "LowCodeLoadOptions.InputFile"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeLoadOptions. Получает и задает путь к файлу шаблона, если необходимо"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodeloadoptions/inputfile/
---
## LowCodeLoadOptions.InputFile property

Получает и задаёт файл (с путём, если необходимо) шаблона.

```csharp
public string InputFile { get; set; }
```

### Примечания

При установке ненулевого и непустого пути в это свойство, ранее установленное значение для [`InputStream`](../inputstream/) будет игнорироваться.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeLoadOptionsPropertyInputFileDemo
    {
        public static void Run()
        {
            // Создайте и сохраните пример файла шаблона
            Workbook templateWorkbook = new Workbook();
            templateWorkbook.Worksheets[0].Cells["A1"].PutValue("Template Value");
            const string templatePath = "LowCodeTemplate.xlsx";
            templateWorkbook.Save(templatePath);

            // Инициализируйте LowCodeLoadOptions и продемонстрируйте свойство InputFile
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            Console.WriteLine("Initial InputFile value: " + loadOptions.InputFile);

            // Установите свойство InputFile для использования нашего шаблона
            loadOptions.InputFile = templatePath;
            Console.WriteLine("Updated InputFile value: " + loadOptions.InputFile);

            // Загрузите книгу, используя указанный файл шаблона
            Workbook workbook = new Workbook(loadOptions.InputFile);
            
            // Измените загруженный шаблон
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A2"].PutValue("Added using InputFile: " + loadOptions.InputFile);

            // Сохранить изменённую книгу
            workbook.Save("PropertyInputFileDemo_Output.xlsx");
        }
    }
}
```

### См. также

* class [LowCodeLoadOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


