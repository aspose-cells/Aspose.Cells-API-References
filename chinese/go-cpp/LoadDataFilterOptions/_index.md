---
title: "LoadDataFilterOptions 枚举"
linktitle: "LoadDataFilterOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "LoadDataFilterOptions 枚举。封装在 Go 中表示 loaddatafilteroptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/loaddatafilteroptions/
---

## LoadDataFilterOptions Enum

表示从模板加载工作簿时过滤数据的选项。

```go

type LoadDataFilterOptions int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [All](./all/) | 加载全部 |
| [CellBlank](./cellblank/) | 加载值为空的单元格 |
| [CellString](./cellstring/) | 加载值为字符串的单元格 |
| [CellNumeric](./cellnumeric/) | 加载值为数值（包括日期时间）的单元格 |
| [CellError](./cellerror/) | 加载值为错误的单元格 |
| [CellBool](./cellbool/) | 加载值为布尔的单元格 |
| [CellValue](./cellvalue/) | 仅加载单元格值（所有值类型） |
| [Formula](./formula/) | 加载单元格公式。 |
| [CellData](./celldata/) | 加载单元格数据，包括值、公式和格式 |
| [Chart](./chart/) | 加载图表 |
| [Drawing](./drawing/) | 绘图对象（包括图表、图片、OleObject 以及所有其他绘图对象） |
| [MergedArea](./mergedarea/) | 加载合并单元格 |
| [ConditionalFormatting](./conditionalformatting/) | 加载条件格式 |
| [DataValidation](./datavalidation/) | 加载数据验证 |
| [PivotTable](./pivottable/) | 加载数据透视表 |
| [Table](./table/) | 加载表格 |
| [Hyperlinks](./hyperlinks/) | 加载超链接 |
| [SheetSettings](./sheetsettings/) | 加载工作表设置 |
| [SheetData](./sheetdata/) | 加载工作表的所有数据，例如单元格数据、设置、对象等。 |
| [BookSettings](./booksettings/) | 加载工作簿的设置 |
| [Settings](./settings/) | 加载工作簿和工作表的设置 |
| [XmlMap](./xmlmap/) | 加载 XmlMap |
| [Structure](./structure/) | 加载工作簿的结构 |
| [Document_Properties](./document_properties/) | 加载文档属性 |
| [DefinedNames](./definednames/) | 加载已定义的 Name 对象 |
| [VBA](./vba/) | 加载 VBA 项目 |
| [Style](./style/) | 加载单元格格式的样式 |
| [Picture](./picture/) | 加载图片 |
| [OleObject](./oleobject/) | 加载 OleObjects |
| [Revision](./revision/) | 加载修订日志 |
