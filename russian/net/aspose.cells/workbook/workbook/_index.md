---
title: "Workbook.Workbook"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор Workbook. Инициализирует новый экземпляр класса Workbook"
type: docs
url: /ru/net/aspose.cells/workbook/workbook/
---
## Workbook() {#constructor}

Инициализирует новый экземпляр класса [`Workbook`](../).

```csharp
public Workbook()
```

### Примечания

Тип формата файла по умолчанию — Xlsx. Если вы хотите создавать файлы других типов, пожалуйста, используйте Workbook(FileFormatType).

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новую рабочую книгу с помощью конструктора
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые данные в ячейки
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Сохраните книгу
            workbook.Save("WorkbookCtorDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook created and saved successfully.");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(FileFormatType) {#constructor_1}

Инициализирует новый экземпляр класса [`Workbook`](../).

```csharp
public Workbook(FileFormatType fileFormatType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileFormatType | FileFormatType | Новый формат файла. |

### Примечания

Тип формата файла по умолчанию — Excel97To2003.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithFileFormatTypeDemo
    {
        public static void Run()
        {
            // Создайте новую книгу с форматом файла XLSX
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Поместите некоторые данные в ячейку A1
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* enum [FileFormatType](../../fileformattype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(LoadOptions) {#constructor_2}

Инициализирует новый пустой экземпляр класса [`Workbook`](../) с параметрами

```csharp
public Workbook(LoadOptions loadOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| loadOptions | LoadOptions | Параметры. |

### См. также

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(string) {#constructor_5}

Инициализирует новый экземпляр класса [`Workbook`](../) и открывает файл.

```csharp
public Workbook(string file)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| файл | String | Имя файла. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithStringDemo
    {
        public static void Run()
        {
            // Путь к каталогу документов.
            string dataDir = "Your Document Directory";

            // Создайте Workbook из существующего файла Excel
            Workbook workbook = new Workbook(dataDir + "example.xlsx");

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Отобразите некоторую информацию о worksheet
            Console.WriteLine("Worksheet Name: " + worksheet.Name);
            Console.WriteLine("Number of Cells: " + worksheet.Cells.Count);

            // Сохраните workbook в формате MHTML
            workbook.Save(dataDir + "output.mht", SaveFormat.MHtml);

            // Создайте другую Workbook из сохранённого файла MHTML
            Workbook workbook2 = new Workbook(dataDir + "output.mht");
            Console.WriteLine("Number of Worksheets in MHTML: " + workbook2.Worksheets.Count);
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(Stream) {#constructor_3}

Инициализирует новый экземпляр класса [`Workbook`](../) и открывает поток.

```csharp
public Workbook(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream | Поток. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSharpctorWithStreamDemo
    {
        public static void Run()
        {
            // Создайте пример файла Excel в памяти
            MemoryStream sampleStream = new MemoryStream();
            Workbook sampleWorkbook = new Workbook();
            sampleWorkbook.Worksheets[0].Cells["A1"].Value = "Sample Data";
            sampleWorkbook.Save(sampleStream, SaveFormat.Xlsx);
            sampleStream.Position = 0; // Reset stream position for reading

            try
            {
                // Создайте новый экземпляр Workbook, используя конструктор Stream
                Workbook workbook = new Workbook(sampleStream);

                // Получить доступ к первому листу
                Worksheet worksheet = workbook.Worksheets[0];

                // Отобразите загруженные данные
                Console.WriteLine($"Loaded data from stream: {worksheet.Cells["A1"].StringValue}");

                // Сохранить книгу в файл
                workbook.Save("WorkbookFromStream.xlsx");
                Console.WriteLine("Workbook saved successfully from stream.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading workbook from stream: {ex.Message}");
            }
            finally
            {
                sampleStream.Dispose();
            }
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(string, LoadOptions) {#constructor_6}

Инициализирует новый экземпляр класса [`Workbook`](../) и открывает файл.

```csharp
public Workbook(string file, LoadOptions loadOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| файл | String | Имя файла. |
| loadOptions | LoadOptions | Параметры загрузки |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithStringLoadOptionsDemo
    {
        public static void Run()
        {
            // Создайте параметры загрузки без LightCellsDataHandler
            LoadOptions loadOptions = new LoadOptions();

            // Инициализируйте workbook с путем к файлу и параметрами загрузки
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);

            // Продемонстрируйте, что workbook загружена, получая количество листов
            Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);
        }
    }
}
```

### См. также

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(Stream, LoadOptions) {#constructor_4}

Инициализирует новый экземпляр класса [`Workbook`](../) и открывает поток.

```csharp
public Workbook(Stream stream, LoadOptions loadOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream | Поток. |
| loadOptions | LoadOptions | Параметры загрузки |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSharpctorWithStreamLoadOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте пример файла Excel в памяти
                byte[] sampleExcelData = GetSampleExcelData();
                MemoryStream stream = new MemoryStream(sampleExcelData);

                // Создайте LoadOptions с конкретными настройками
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
                loadOptions.MemorySetting = MemorySetting.MemoryPreference;

                // Создайте экземпляр Workbook, используя #ctor с Stream и LoadOptions
                Workbook workbook = new Workbook(stream, loadOptions);

                // Отобразите базовую информацию о загруженном workbook
                Console.WriteLine("Workbook loaded successfully!");
                Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);
                Console.WriteLine("File format: " + workbook.FileFormat);

                // Получить доступ к первому листу
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine("First worksheet name: " + worksheet.Name);

                // Отобразить содержимое ячейки, если оно доступно
                if (worksheet.Cells["A1"].Value != null)
                {
                    Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value.ToString());
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading workbook: {ex.Message}");
            }
        }

        private static byte[] GetSampleExcelData()
        {
            // Создать простой файл Excel в памяти для демонстрации
            using (MemoryStream ms = new MemoryStream())
            {
                Workbook tempWorkbook = new Workbook();
                tempWorkbook.Worksheets[0].Cells["A1"].PutValue("Sample Data");
                tempWorkbook.Worksheets[0].Cells["B1"].PutValue("Created for demo");
                tempWorkbook.Save(ms, SaveFormat.Xlsx);
                return ms.ToArray();
            }
        }
    }
}
```

### См. также

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


