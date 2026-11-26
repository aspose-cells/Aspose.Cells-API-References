---
title: "Класс StreamProviderOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.StreamProviderOptions. Представляет параметры потока"
type: docs
url: /ru/net/aspose.cells/streamprovideroptions/
---
## StreamProviderOptions class

Представляет параметры потока.

```csharp
public class StreamProviderOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [StreamProviderOptions](streamprovideroptions/#constructor)() | Инициализирует новый экземпляр класса `StreamProviderOptions`. |
| [StreamProviderOptions](streamprovideroptions/#constructor_1)(ResourceLoadingType, string) | Инициализирует новый экземпляр класса `StreamProviderOptions`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CustomPath](../../aspose.cells/streamprovideroptions/custompath/) { get; set; } | Пользовательский путь (URL), сохранённый в сгенерированном HTML-файле для ссылочного источника. Если пользователь не задаёт его, будет использован DefaultPath. Например, данные листа будут сохранены пользователем в d:/sheet001.htm, URL, используемый в основном HTML-файле, должен быть "d:/sheet001.htm" или иной допустимый относительный путь, доступный из основного HTML-файла. |
| [DefaultPath](../../aspose.cells/streamprovideroptions/defaultpath/) { get; } | Путь по умолчанию (URL), сохраненный в сгенерированном html‑файле для указанного источника. Например, данные листа, сохранённые в xxx_files/sheet001.htm, URL, используемый в основном html‑файле, должен выглядеть так \"src=\"xxx_files/sheet001.htm\"\" |
| [ResourceLoadingType](../../aspose.cells/streamprovideroptions/resourceloadingtype/) { get; set; } | Получает и задает тип загружаемого ресурса. |
| [Stream](../../aspose.cells/streamprovideroptions/stream/) { get; set; } | Получает/задаёт поток |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassStreamProviderOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Создать StreamProviderOptions
            StreamProviderOptions options = new StreamProviderOptions();
            
            // Установить поток памяти для демонстрации
            options.Stream = new MemoryStream();
            
            // Использовать поток (пример: сохранить книгу в поток)
            workbook.Save(options.Stream, SaveFormat.Xlsx);
            
            // Продемонстрировать закрытие потока
            CloseStream(options);
        }

        public static void CloseStream(StreamProviderOptions options)
        {
            if (options.Stream != null)
            {
                options.Stream.Close();
                options.Stream = null;
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


