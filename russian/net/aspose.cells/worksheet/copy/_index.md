---
title: "Worksheet.Copy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Копирует содержимое и форматы из другого рабочего листа"
type: docs
url: /ru/net/aspose.cells/worksheet/copy/
---
## Copy(Worksheet) {#copy}

Копирует содержимое и форматы из другого листа.

```csharp
public void Copy(Worksheet sourceSheet)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceSheet | Worksheet | Исходный рабочий лист. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCopyWithWorksheetDemo
    {
        public static void Run()
        {
            // Создайте исходную книгу с примерными данными
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Worksheet");
            
            // Создайте целевую книгу
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Скопировать исходный рабочий лист в целевой рабочий лист
            destSheet.Copy(sourceSheet);
            
            // Сохранить результат
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Worksheet, CopyOptions) {#copy_1}

Копирует содержимое и форматы из другого листа.

```csharp
public void Copy(Worksheet sourceSheet, CopyOptions copyOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceSheet | Worksheet | Исходный рабочий лист. |
| copyOptions | CopyOptions |  |

### Примечания

Вы можете копировать данные из другого рабочего листа в том же файле или из другого файла. Однако этот метод не поддерживает копирование графических объектов, таких как комментарии, изображения и диаграммы.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCopyWithWorksheetCopyOptionsDemo
    {
        public static void Run()
        {
            // Создайте исходную книгу с образцовыми данными
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Name = "SourceSheet";
            srcSheet.Cells["A1"].PutValue("Source Data");

            // Создайте целевую книгу
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            destSheet.Name = "DestinationSheet";

            // Настроить параметры копирования
            CopyOptions options = new CopyOptions();
            options.ReferToDestinationSheet = true;

            // Копировать лист с параметрами
            srcSheet.Copy(destSheet, options);

            // Проверить операцию копирования
            Console.WriteLine("Copied cell value: " + destSheet.Cells["A1"].StringValue);
            
            // Сохранить результат
            destWorkbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [CopyOptions](../../copyoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


