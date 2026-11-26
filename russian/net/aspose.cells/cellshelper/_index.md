---
title: "Класс CellsHelper"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.CellsHelper. Предоставляет вспомогательные функции"
type: docs
url: /ru/net/aspose.cells/cellshelper/
---
## CellsHelper class

Предоставляет вспомогательные функции.

```csharp
public class CellsHelper
```

## Свойства

| Имя | Описание |
| --- | --- |
| static [AltStartPath](../../aspose.cells/cellshelper/altstartpath/) { get; set; } | Получает или задает альтернативный путь запуска, на который ссылаются некоторые внешние формульные ссылки. |
| static [CustomImplementationFactory](../../aspose.cells/cellshelper/customimplementationfactory/) { get; set; } | Получает или задает фабрику для создания экземпляров со специальной реализацией. |
| static [DPI](../../aspose.cells/cellshelper/dpi/) { get; set; } | Получает DPI машины. |
| static [IsCloudPlatform](../../aspose.cells/cellshelper/iscloudplatform/) { get; set; } | Пожалуйста, установите это свойство в значение True при работе на облачной платформе, такой как: Azure, AWSLambda и т.д. |
| static [LibraryPath](../../aspose.cells/cellshelper/librarypath/) { get; set; } | Получает или задает путь к библиотеке, на который ссылаются некоторые внешние формульные ссылки. |
| static [SignificantDigits](../../aspose.cells/cellshelper/significantdigits/) { get; set; } | (**Obsolete.**) Получает и задает количество значимых цифр. Значение по умолчанию — 17. |
| static [SignificantDigitsType](../../aspose.cells/cellshelper/significantdigitstype/) { get; set; } | Получает и задает тип значимых цифр по умолчанию для вывода числовых значений. Значение по умолчанию — G17. |
| static [StartupPath](../../aspose.cells/cellshelper/startuppath/) { get; set; } | Получает или задает путь запуска, на который ссылаются некоторые внешние формульные ссылки. |

## Методы

| Имя | Описание |
| --- | --- |
| static [AddAddInFunction](../../aspose.cells/cellshelper/addaddinfunction/)(string, int, int, ParameterType[], ParameterType) | (**Obsolete.**) Добавить функцию надстройки. |
| static [CellIndexToName](../../aspose.cells/cellshelper/cellindextoname/)(int, int) | Получает имя ячейки в соответствии с её индексами строки и столбца. |
| static [CellNameToIndex](../../aspose.cells/cellshelper/cellnametoindex/)(string, out int, out int) | Получает индексы строки и столбца ячейки в соответствии с её именем. |
| static [ColumnIndexToName](../../aspose.cells/cellshelper/columnindextoname/)(int) | Получает имя столбца в соответствии с индексом столбца. |
| static [ColumnNameToIndex](../../aspose.cells/cellshelper/columnnametoindex/)(string) | Получает индекс столбца в соответствии с именем столбца. |
| static [ConvertA1FormulaToR1C1](../../aspose.cells/cellshelper/converta1formulator1c1/)(string, int, int) | (**Obsolete.**) Преобразует формулу A1 ячейки в формулу r1c1. |
| static [ConvertR1C1FormulaToA1](../../aspose.cells/cellshelper/convertr1c1formulatoa1/)(string, int, int) | (**Obsolete.**) Преобразует формулу r1c1 ячейки в формулу A1. |
| static [CreateSafeSheetName](../../aspose.cells/cellshelper/createsafesheetname/#createsafesheetname)(string) | Проверяет указанное имя листа и при необходимости создает корректное. Если указанное имя листа соответствует правилам имен листов Excel, возвращает его. В противном случае строка будет усечена, если её длина превышает ограничение, а недопустимые символы будут заменены на ' ', затем возвращается восстановленное значение строки. |
| static [CreateSafeSheetName](../../aspose.cells/cellshelper/createsafesheetname/#createsafesheetname_1)(string, char) | Проверяет указанное имя листа и при необходимости создает корректное. Если указанное имя листа соответствует правилам имен листов Excel, возвращает его. В противном случае строка будет усечена, если её длина превышает ограничение, а недопустимые символы будут заменены заданным символом, затем возвращается восстановленное значение строки. |
| static [GetCacheFolder](../../aspose.cells/cellshelper/getcachefolder/)() | Получает папку для временных файлов, которые могут использоваться в качестве кэша данных. |
| static [GetDateTimeFromDouble](../../aspose.cells/cellshelper/getdatetimefromdouble/)(double, bool) | Преобразует значение double в значение даты и времени. |
| static [GetDoubleFromDateTime](../../aspose.cells/cellshelper/getdoublefromdatetime/)(DateTime, bool) | Преобразует дату и время в значение double. |
| static [GetTextWidth](../../aspose.cells/cellshelper/gettextwidth/)(string, Font, double) | Получить ширину текста в единицах точек. |
| static [GetUsedColors](../../aspose.cells/cellshelper/getusedcolors/)(Workbook) | Получает все используемые цвета в рабочей книге. |
| static [GetVersion](../../aspose.cells/cellshelper/getversion/)() | Получить версию выпуска. |
| static [MergeFiles](../../aspose.cells/cellshelper/mergefiles/)(string[], string, string) | Объединяет несколько больших файлов xls в один файл xls. |
| static [NeedQuoteInFormula](../../aspose.cells/cellshelper/needquoteinformula/)(string) | Указывает, следует ли заключать имя листа в одинарные кавычки |
| static [RowIndexToName](../../aspose.cells/cellshelper/rowindextoname/)(int) | Получает имя строки в соответствии с индексом строки. |
| static [RowNameToIndex](../../aspose.cells/cellshelper/rownametoindex/)(string) | Получает индекс строки в соответствии с её именем. |
| static [SetCacheFolder](../../aspose.cells/cellshelper/setcachefolder/)(string) | Устанавливает папку для временных файлов, которые могут использоваться в качестве кэша данных. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperDemo
    {
        public static void CellsHelperExample()
        {
            // Настройка свойств CellsHelper
            CellsHelper.SignificantDigits = 15;
            CellsHelper.DPI = 96.0;
            CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
            CellsHelper.AltStartPath = "D:\\Aspose\\Cells";
            CellsHelper.LibraryPath = "E:\\Aspose\\Cells\\Library";
            CellsHelper.IsCloudPlatform = true;

            // Предполагая, что CustomImplementationFactory уже определён и создан в другом месте
            CellsHelper.CustomImplementationFactory = new CustomImplementationFactory();

            // Продемонстрировано использование свойств CellsHelper
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
            Console.WriteLine("DPI: " + CellsHelper.DPI);
            Console.WriteLine("Startup Path: " + CellsHelper.StartupPath);
            Console.WriteLine("Alternate Startup Path: " + CellsHelper.AltStartPath);
            Console.WriteLine("Library Path: " + CellsHelper.LibraryPath);
            Console.WriteLine("Is Cloud Platform: " + CellsHelper.IsCloudPlatform);

            // Пример использования CustomImplementationFactory
            var memoryStream = CellsHelper.CustomImplementationFactory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created with CustomImplementationFactory: " + (memoryStream != null));

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


