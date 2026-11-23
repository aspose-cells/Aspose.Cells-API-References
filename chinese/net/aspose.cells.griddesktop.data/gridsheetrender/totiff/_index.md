---
title: "GridSheetRender.ToTiff"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "GridSheetRender 方法。将整个工作表渲染为 Tiff 图像并输出到流"
type: docs
url: /zh/net/aspose.cells.griddesktop.data/gridsheetrender/totiff/
---
## ToTiff(Stream) {#totiff}

将整个工作表渲染为 Tiff 图像并输出到流。

```csharp
public void ToTiff(Stream stream)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | Stream | 输出图像的流 |

### 另请参见

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToTiff(string) {#totiff_1}

将整个工作表渲染为 Tiff 图像并保存到文件。

```csharp
public void ToTiff(string filename)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件名 | String | 输出图像的文件名 |

### 示例

以下代码将第一张工作表的所有页面输出为 Tiff 图像。

```csharp
//加载带有图像的源文件。
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

//设置输出图像类型。
imgOpt.SaveFormat = SaveFormat.Tiff;

//渲染第一张工作表。
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

//将工作表的所有页面输出为 Tiff 图像。
sr.ToTiff("output.tiff");
```

### 另请参见

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


