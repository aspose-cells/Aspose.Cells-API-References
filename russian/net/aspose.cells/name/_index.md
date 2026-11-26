---
title: "Класс Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Name. Представляет определённое имя для диапазона ячеек"
type: docs
url: /ru/net/aspose.cells/name/
---
## Name class

Представляет определённое имя диапазона ячеек.

```csharp
public class Name
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Comment](../../aspose.cells/name/comment/) { get; set; } | Получает и задаёт комментарий к имени. Применяется только для Excel 2007 и более новых версий. |
| [FullText](../../aspose.cells/name/fulltext/) { get; } | Получает полный текст имени объекта с настройкой области. |
| [IsReferred](../../aspose.cells/name/isreferred/) { get; } | Указывает, используется ли это имя в других формулах. |
| [IsVisible](../../aspose.cells/name/isvisible/) { get; set; } | Указывает, видимо ли имя. |
| [R1C1RefersTo](../../aspose.cells/name/r1c1refersto/) { get; set; } | Получает или задаёт ссылку R1C1 для `Name`. |
| [RefersTo](../../aspose.cells/name/refersto/) { get; set; } | Возвращает или задаёт формулу, к которой определено имя, начиная со знака равенства. |
| [SheetIndex](../../aspose.cells/name/sheetindex/) { get; set; } | Указывает, принадлежит ли это имя книге Workbook или листу Worksheet. 0 = глобальное имя, иначе индекс листа (нумерация с единицы). |
| [Text](../../aspose.cells/name/text/) { get; set; } | Получает текст имени объекта. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetRange](../../aspose.cells/name/getrange/#getrange)() | Получает диапазон, если это имя ссылается на диапазон. |
| [GetRange](../../aspose.cells/name/getrange/#getrange_1)(bool) | Получает диапазон, если это имя ссылается на диапазон |
| [GetRange](../../aspose.cells/name/getrange/#getrange_2)(int, int, int) | Получает диапазон, если это имя ссылается на диапазон. Если ссылка этого имени не абсолютна, диапазон может различаться для разных ячеек. |
| [GetRanges](../../aspose.cells/name/getranges/#getranges)() | Получает все диапазоны, на которые ссылается это имя. |
| [GetRanges](../../aspose.cells/name/getranges/#getranges_1)(bool) | Получает все диапазоны, на которые ссылается это имя. |
| [GetReferredAreas](../../aspose.cells/name/getreferredareas/)(bool) | Получает все ссылки, на которые ссылается это имя. |
| [GetRefersTo](../../aspose.cells/name/getrefersto/#getrefersto)(bool, bool) | Получить ссылку этого Name. |
| [GetRefersTo](../../aspose.cells/name/getrefersto/#getrefersto_1)(bool, bool, int, int) | Получить ссылку этого Name на основе указанной ячейки. |
| [SetRefersTo](../../aspose.cells/name/setrefersto/)(string, bool, bool) | Задать ссылку этого Name. |
| override [ToString](../../aspose.cells/name/tostring/)() | Возвращает строку, представляющую текущий объект Range. |

### Примеры

```csharp

[C#]

//Создание объекта Workbook
Workbook workbook = new Workbook();
//Доступ к первому листу в файле Excel
Worksheet worksheet = workbook.Worksheets[0];
//Создание именованного диапазона
Range range = worksheet.Cells.CreateRange("B4", "G14");
//Установка имени именованного диапазона
range.Name = "TestRange";
//Сохранение измененного файла Excel в формате по умолчанию (то есть Excel 2000)
workbook.Save("output.xls");   

[Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Accessing the first worksheet in the Excel file
Dim worksheet As Worksheet = workbook.Worksheets(0)
'Creating a named range
Dim range As Range = worksheet.Cells.CreateRange("B4", "G14")
'Setting the name of the named range
range.Name = "TestRange"
'Saving the modified Excel file in default (that is Excel 2000) format
workbook.Save("output.xls")
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


