---
title: GridJsWorkbook
second_title: Aspose.Cells for .NET API 参考
description: 表示 GridJs 的主要入口类
type: docs
weight: 80
url: /zh/net/aspose.cells.gridjs/gridjsworkbook/
---
## GridJsWorkbook class

表示 GridJs 的主要入口类

```csharp
public class GridJsWorkbook
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [GridJsWorkbook](gridjsworkbook)() | 默认构造函数。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Settings](../../aspose.cells.gridjs/gridjsworkbook/settings) { get; set; } | 表示工作簿设置。 |
| [WarningCallback](../../aspose.cells.gridjs/gridjsworkbook/warningcallback) { get; set; } | 获取或设置导入文件的警告回调。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [CopyImageOrShape](../../aspose.cells.gridjs/gridjsworkbook/copyimageorshape)(string, string) | 在工作表中复制图像或形状 |
| [ErrorJson](../../aspose.cells.gridjs/gridjsworkbook/errorjson)(string) | 返回错误信息 |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson#exporttojson)() | 从工作簿获取 json |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson#exporttojson_1)(string) | 从工作簿中获取 json |
| [ExportToJsonStringBuilder](../../aspose.cells.gridjs/gridjsworkbook/exporttojsonstringbuilder)(string) | 从工作簿中获取 json |
| [GetJsonByUid](../../aspose.cells.gridjs/gridjsworkbook/getjsonbyuid)(string, string) | 通过 uid 从缓存中获取 json |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_3)(string) | 从 excel 文件导入。 |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile)(Workbook) | 从工作簿导入。 |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_1)(Stream, GridLoadFormat) | 从 excel 文件流中导入。必须提供 loadformat 并且可以设置 GridJsWorkbook.CacheImp 来实现流缓存 |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_7)(string, string) | 从 excel 文件导入。 |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_4)(string, Workbook) | 从 excel 文件导入。 |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_2)(Stream, GridLoadFormat, string) | 从 excel 文件流中导入。必须提供 loadformat 并且可以设置 GridJsWorkbook.CacheImp 来实现流缓存 |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_5)(string, Stream, GridLoadFormat) | 从 excel 文件流中导入。必须提供 loadformat 并且可以设置 GridJsWorkbook.CacheImp 来实现流缓存 |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_8)(string, string, string) | 从 excel 文件导入。 |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_6)(string, Stream, GridLoadFormat, string) | 从 excel 文件流中导入。必须提供 loadformat 并且可以设置 GridJsWorkbook.CacheImp 来实现流缓存 |
| [ImportExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/importexcelfilefromjson)(string) | 从 json 导入文件 |
| [InsertImage](../../aspose.cells.gridjs/gridjsworkbook/insertimage)(string, string, Stream, string) | 在工作表中插入图像 |
| [MergeExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/mergeexcelfilefromjson)(string, string) | 将样式更新应用到缓存文件 |
| [SaveToCacheWithFileName](../../aspose.cells.gridjs/gridjsworkbook/savetocachewithfilename)(string, string, string) | 将工作表保存到缓存中，保存格式基于 filename 的文件扩展名。 |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile#savetoexcelfile)(Stream) | 根据原始文件格式将工作表保存到 sream 中。 |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile#savetoexcelfile_1)(string) | 将工作表保存到文件路径，如果文件有扩展名，则保存格式基于文件扩展名。 |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml#savetohtml)(Stream) | 将工作表保存到 sream，保存格式为 html |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml#savetohtml_1)(string) | 将工作表保存到文件路径，保存格式为 html |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf#savetopdf)(Stream) | 将工作表保存到 sream，保存格式为 pdf |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf#savetopdf_1)(string) | 将工作表保存到文件路径，保存格式为pdf |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx#savetoxlsx)(Stream) | 将工作表保存到 sream，保存格式为 xlsx |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx#savetoxlsx_1)(string) | 将工作表保存到文件路径，保存格式为 xlsx |
| [SetInterruptMonitorForLoad](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforload)(GridInterruptMonitor, int) | 为工作簿的加载操作设置 InterruptMonitor |
| [SetInterruptMonitorForSave](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforsave)(GridInterruptMonitor) | 为工作簿的保存操作设置 InterruptMonitor |
| [UpdateCell](../../aspose.cells.gridjs/gridjsworkbook/updatecell)(string, string) | 做更新操作 |
| static [GetGridLoadFormat](../../aspose.cells.gridjs/gridjsworkbook/getgridloadformat)(string) | 通过文件扩展名获取 GridLoadFormat |
| static [GetImageStream](../../aspose.cells.gridjs/gridjsworkbook/getimagestream)(string, string) | 从工作簿获取图像流 |
| static [GetImageUrl](../../aspose.cells.gridjs/gridjsworkbook/getimageurl)(string, string, string) | 获取图像 URL |
| static [GetUidForFile](../../aspose.cells.gridjs/gridjsworkbook/getuidforfile)(string) | 生成文件的uid |

## 字段

| 姓名 | 描述 |
| --- | --- |
| static [CacheImp](../../aspose.cells.gridjs/gridjsworkbook/cacheimp) | 自定义实现缓存存储，如果要以流的方式存储缓存，需要设置并实现 |
| static [CalculateEngine](../../aspose.cells.gridjs/gridjsworkbook/calculateengine) | 计算引擎的自定义实现，如果要进行自定义计算，需要设置并实现 |

### 也可以看看

* 命名空间 [Aspose.Cells.GridJs](../../aspose.cells.gridjs)
* 部件 [Aspose.Cells.GridJs](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridJs.dll -->
