---
title: LoadFilter
second_title: Aspose.Cells for .NET API 参考
description: 表示从模板加载工作簿时提供加载数据选项的过滤器
type: docs
weight: 3980
url: /zh/net/aspose.cells/loadfilter/
---
## LoadFilter class

表示从模板加载工作簿时提供加载数据选项的过滤器。

```csharp
public class LoadFilter
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [LoadFilter](loadfilter#constructor)() | 使用默认过滤器选项 LoadDataFilterOptions.All. 构造一个 LoadFilter |
| [LoadFilter](loadfilter#constructor_1)(LoadDataFilterOptions) | 使用给定的过滤器选项构造一个 LoadFilter。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [LoadDataFilterOptions](../../aspose.cells/loadfilter/loaddatafilteroptions) { get; set; } | 表示应该加载哪些数据的过滤器选项。 |
| virtual [SheetsInLoadingOrder](../../aspose.cells/loadfilter/sheetsinloadingorder) { get; } | 指定要加载的工作表（索引）和顺序。 默认为空，表示在模板文件中按默认顺序加载所有工作表。 如果不为空且某些工作表的索引不在返回的数组中，则工作表不会被加载。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| virtual [StartSheet](../../aspose.cells/loadfilter/startsheet)(Worksheet) | 在加载给定的工作表之前准备过滤器选项。 用户的 LoadFilter 实现可以在这里更改 LoadDataFilterOptions 以表示如何为此工作表加载数据。 |

### 评论

用户可以指定过滤器选项或实现自己的LoadFilter来指定如何加载数据。

### 例子

以下示例显示如何根据工作表的属性确定过滤器选项。

```csharp
[C#]
Workbook wb = new Workbook(template, new LoadOptions() { LoadFilter = new LoadFilterSheet() });
//自定义LoadFilter实现
class LoadFilterSheet : LoadFilter
{
    public override void StartSheet(Worksheet sheet) 
    {
        if (sheet.Name == "Sheet1")
        {
            LoadDataFilterOptions = Aspose.Cells.LoadDataFilterOptions.All;
        }
        else
        {
            LoadDataFilterOptions = Aspose.Cells.LoadDataFilterOptions.None;
        }
    }
}
```

### 也可以看看

* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
