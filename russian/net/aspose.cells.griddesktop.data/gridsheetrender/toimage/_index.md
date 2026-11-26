---
title: "GridSheetRender.ToImage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridSheetRender. Отрисовать определённую страницу в объект Graphics"
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridsheetrender/toimage/
---
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}

Отрисовать определённую страницу в объект Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | указать, какая страница будет конвертирована |
| g | Графика | Объект, в который нужно отрисовать. |
| x | Single | Координата X (в пикселях) верхнего левого угла отрисованной страницы. |
| y | Single | Координата Y (в пикселях) верхнего левого угла отрисованной страницы. |
| ширина | Single | Максимальная ширина (в пикселях), которую может занимать отрисованная страница. |
| высота | Single | Максимальная высота (в пикселях), которую может занимать отрисованная страница. |

### См. также

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, Graphics, float, float) {#toimage_1}

Отрисовать определённую страницу в объект Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | указать, какая страница будет конвертирована |
| g | Графика | Объект, в который нужно отрисовать. |
| x | Single | Координата X (в пикселях) верхнего левого угла отрисованной страницы. |
| y | Single | Координата Y (в пикселях) верхнего левого угла отрисованной страницы. |

### См. также

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, string) {#toimage_4}

Отрисовать определённую страницу в файл.

```csharp
public void ToImage(int pageIndex, string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | указать, какая страница будет конвертирована |
| fileName | String | имя файла выходного изображения |

### Примеры

Следующий код выводит первую страницу первого листа в png‑изображение.

```csharp
//загрузите исходный файл с изображениями.
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

//Установите тип выходного изображения.
imgOpt.ImageType = ImageType.Png;

//Отобразите первый лист.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

//Выведите первую страницу листа в изображение.
sr.ToImage(0, "output.png");
```

### См. также

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, Stream) {#toimage_3}

Отрисовать определённую страницу в поток.

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | указать, какая страница будет конвертирована |
| поток | Stream | поток выходного изображения |

### См. также

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int) {#toimage}

Отрисовать определённую страницу в объект Bitmap.

```csharp
public Bitmap ToImage(int pageIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | указать, какая страница будет конвертирована |

### Возвращаемое значение

объект bitmap страницы

### См. также

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


