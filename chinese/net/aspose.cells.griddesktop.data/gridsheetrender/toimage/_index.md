---
title: "GridSheetRender.ToImage"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "GridSheetRender 方法。将特定页面渲染到 Graphics"
type: docs
url: /zh/net/aspose.cells.griddesktop.data/gridsheetrender/toimage/
---
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}

将指定页面渲染到 Graphics。

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pageIndex | Int32 | 指示要转换的页面 |
| g | Graphics | 要渲染到的对象。 |
| x | Single | 渲染页面左上角的 X 坐标（像素）。 |
| y | Single | 渲染页面左上角的 Y 坐标（像素）。 |
| 宽度 | Single | 渲染页面可占用的最大宽度（像素）。 |
| height | Single | 渲染页面可占用的最大高度（像素）。 |

### 另请参见

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, Graphics, float, float) {#toimage_1}

将指定页面渲染到 Graphics。

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pageIndex | Int32 | 指示要转换的页面 |
| g | Graphics | 要渲染到的对象。 |
| x | Single | 渲染页面左上角的 X 坐标（像素）。 |
| y | Single | 渲染页面左上角的 Y 坐标（像素）。 |

### 另请参见

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, string) {#toimage_4}

将指定页面渲染到文件中。

```csharp
public void ToImage(int pageIndex, string fileName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pageIndex | Int32 | 指示要转换的页面 |
| fileName | String | 输出图像的文件名 |

### 示例

以下代码将第一张工作表的第一页输出为 PNG 图像。

```csharp
//加载带有图像的源文件。
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

//设置输出图像类型。
imgOpt.ImageType = ImageType.Png;

//渲染第一张工作表。
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

//将工作表的第一页输出为图像。
sr.ToImage(0, "output.png");
```

### 另请参见

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, Stream) {#toimage_3}

将指定页面渲染到流中。

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pageIndex | Int32 | 指示要转换的页面 |
| stream | Stream | 输出图像的流 |

### 另请参见

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int) {#toimage}

将指定页面渲染为 Bitmap 对象。

```csharp
public Bitmap ToImage(int pageIndex)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pageIndex | Int32 | 指示要转换的页面 |

### 返回值

页面的位图对象

### 另请参见

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


