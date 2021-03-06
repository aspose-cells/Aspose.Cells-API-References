---
title: ToTiff
second_title: Справочник по Aspose.Cells для .NET API
description: Визуализация всего рабочего листа в виде изображения Tiff для потоковой передачи.
type: docs
weight: 80
url: /ru/net/aspose.cells.rendering/sheetrender/totiff/
---
## ToTiff(Stream) {#totiff}

Визуализация всего рабочего листа в виде изображения Tiff для потоковой передачи.

```csharp
public void ToTiff(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | поток выходного изображения |

### Смотрите также

* class [SheetRender](../../sheetrender)
* пространство имен [Aspose.Cells.Rendering](../../sheetrender)
* сборка [Aspose.Cells](../../../)

---

## ToTiff(string) {#totiff_1}

Визуализация всего рабочего листа в виде изображения Tiff в файл.

```csharp
public void ToTiff(string filename)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filename | String | имя файла выходного изображения |

### Примеры

Следующий код выводит все страницы первого листа в изображение Tiff.

```csharp
//загрузить исходный файл с изображениями.
rkbook wb = new Workbook("Book1.xlsx");

ageOrPrintOptions imgOpt = new ImageOrPrintOptions();

//установить тип выходного изображения.
gOpt.SaveFormat = SaveFormat.Tiff;

//рендерим первый лист.
eetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

//выводим все страницы листа в Tiff image.
.ToTiff("output.tiff");
```

### Смотрите также

* class [SheetRender](../../sheetrender)
* пространство имен [Aspose.Cells.Rendering](../../sheetrender)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
