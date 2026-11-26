---
title: "GridSheetRender.ToTiff"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridSheetRender. Отображает весь рабочий лист как Tiff‑изображение в поток."
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridsheetrender/totiff/
---
## ToTiff(Stream) {#totiff}

Отрисовать весь лист как изображение Tiff в поток.

```csharp
public void ToTiff(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream | поток выходного изображения |

### См. также

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToTiff(string) {#totiff_1}

Отрисовать весь лист как изображение Tiff в файл.

```csharp
public void ToTiff(string filename)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| имя файла | String | имя файла выходного изображения |

### Примеры

Следующий код выводит все страницы первого листа в Tiff‑изображение.

```csharp
//загрузите исходный файл с изображениями.
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

//Установите тип выходного изображения.
imgOpt.SaveFormat = SaveFormat.Tiff;

//Отобразите первый лист.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

//Выведите все страницы листа в Tiff‑изображение.
sr.ToTiff("output.tiff");
```

### См. также

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


