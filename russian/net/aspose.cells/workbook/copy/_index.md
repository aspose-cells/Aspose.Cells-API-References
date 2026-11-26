---
title: "Workbook.Copy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Копирует другой объект Workbook"
type: docs
url: /ru/net/aspose.cells/workbook/copy/
---
## Copy(Workbook, CopyOptions) {#copy_1}

Копирует другой объект Workbook.

```csharp
public void Copy(Workbook source, CopyOptions copyOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| источник | Рабочая книга | Исходный объект Workbook. |
| copyOptions | CopyOptions | Параметры копирования другой книги. |

### Примечания

Клонировать файл Excel очень просто.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyWithWorkbookCopyOptionsDemo
    {
        public static void Run()
        {
            // Исходная книга с макросами
            Workbook sourceWorkbook = new Workbook("source_with_macros.xlsm");
            
            // Книга назначения (пустая или существующая)
            Workbook destWorkbook = new Workbook();
            
            // Настроить параметры копирования для сохранения макросов
            CopyOptions options = new CopyOptions();
            options.KeepMacros = true;
            
            // Скопировать содержимое из исходной книги в книгу назначения
            sourceWorkbook.Copy(destWorkbook, options);
            
            // Сохранить результат
            destWorkbook.Save("output_with_macros.xlsm");
        }
    }
}
```

### См. также

* class [CopyOptions](../../copyoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Workbook) {#copy}

Копирует данные из исходного объекта Workbook.

```csharp
public void Copy(Workbook source)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| источник | Рабочая книга | Исходный объект Workbook. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyWithWorkbookDemo
    {
        public static void Run()
        {
            // Пути к исходному и выходному файлам
            string sourceFile = "source.xlsx";
            string outputFile = "output.xlsx";

            // Загрузить исходную книгу
            Workbook sourceWorkbook = new Workbook(sourceFile);

            // Создайте новую книгу и скопируйте содержимое из источника
            Workbook destinationWorkbook = new Workbook();
            destinationWorkbook.Copy(sourceWorkbook);

            // Сохраните скопированную книгу
            destinationWorkbook.Save(outputFile);
            
            Console.WriteLine("Workbook copied successfully.");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


