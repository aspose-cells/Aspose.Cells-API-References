---
title: "类 HtmlTableLoadOptionCollection"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.HtmlTableLoadOptionCollection 类。表示导入 HTML 时的表格选项"
type: docs
url: /zh/net/aspose.cells/htmltableloadoptioncollection/
---
## HtmlTableLoadOptionCollection class

表示导入 HTML 时的表格选项。

```csharp
public class HtmlTableLoadOptionCollection : CollectionBase<HtmlTableLoadOption>
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [HtmlTableLoadOptionCollection](htmltableloadoptioncollection/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/htmltableloadoptioncollection/item/) { get; } | 获取指定索引处的[`HtmlTableLoadOption`](../htmltableloadoption/) 元素。 |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [TableToListObject](../../aspose.cells/htmltableloadoptioncollection/tabletolistobject/) { get; set; } | 指示是否从导入的表生成列表对象。默认值为 false。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add)(HtmlTableLoadOption) | (**Obsolete.**) 向此集合添加一个 HtmlTableLoadOption。 |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_1)(int) | 向列表添加一个 HtmlTableLoadOption。 |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_4)(string) | 向列表添加一个 HtmlTableLoadOption。 |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_2)(int, int) | 向列表添加一个 HtmlTableLoadOption。 |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_5)(string, int) | 向列表添加一个 HtmlTableLoadOption。 |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_3)(int, int, int) | 向列表添加一个 HtmlTableLoadOption。 |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_6)(string, int, int) | 向列表添加一个 HtmlTableLoadOption。 |
| [AddTableLoadOption](../../aspose.cells/htmltableloadoptioncollection/addtableloadoption/)(HtmlTableLoadOption) | 向此集合添加一个 HtmlTableLoadOption。 |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HtmlTableLoadOption) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HtmlTableLoadOption, IComparer&lt;HtmlTableLoadOption&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, HtmlTableLoadOption, IComparer&lt;HtmlTableLoadOption&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(HtmlTableLoadOption) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HtmlTableLoadOption[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HtmlTableLoadOption[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, HtmlTableLoadOption[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlTableLoadOptionCollectionDemo
    {
        public static void HtmlTableLoadOptionCollectionExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 创建 HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // 访问 HtmlTableLoadOptionCollection 实例
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // 设置 TableToListObject 属性
            tableLoadOptions.TableToListObject = true;

            // 按表索引添加新的 HtmlTableLoadOption
            int index1 = tableLoadOptions.Add(0);

            // 按表 ID 添加新的 HtmlTableLoadOption
            int index2 = tableLoadOptions.Add("tableId");

            // 按表索引和目标工作表索引添加新的 HtmlTableLoadOption
            int index3 = tableLoadOptions.Add(1, 1);

            // 按表 ID 和目标工作表索引添加新的 HtmlTableLoadOption
            int index4 = tableLoadOptions.Add("tableId2", 2);

            // 按表索引、目标工作表索引和原始工作表索引添加新的 HtmlTableLoadOption
            int index5 = tableLoadOptions.Add(2, 2, 0);

            // 按表 ID、目标工作表索引和原始工作表索引添加新的 HtmlTableLoadOption
            int index6 = tableLoadOptions.Add("tableId3", 3, 1);

            // 在特定索引处访问 HtmlTableLoadOption
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // 设置 HtmlTableLoadOption 的属性
            option.TableIndex = 0;
            option.Id = "tableId";
            option.Name = "TableName";
            option.OriginalSheetIndex = 0;
            option.TargetSheetIndex = 1;
            option.TableToListObject = true;

            // 使用加载选项将 HTML 文件加载到工作簿中
            workbook = new Workbook("HtmlTableLoadOptionCollectionExample_original.html", loadOptions);

            // 保存工作簿
            workbook.Save("HtmlTableLoadOptionCollectionExample.xlsx");

            return;
        }
    }
}
```

### 另请参见

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [HtmlTableLoadOption](../htmltableloadoption/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


