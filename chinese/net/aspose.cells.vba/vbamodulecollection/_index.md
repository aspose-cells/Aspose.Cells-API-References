---
title: VbaModuleCollection
second_title: Aspose.Cells for .NET API 参考
description: 代表列表VbaModule./vbamodule
type: docs
weight: 6250
url: /zh/net/aspose.cells.vba/vbamodulecollection/
---
## VbaModuleCollection class

代表列表[`VbaModule`](../vbamodule)

```csharp
public class VbaModuleCollection : CollectionBase<VbaModule>
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.vba/vbamodulecollection/item) { get; } | 获取[`VbaModule`](../vbamodule)在索引列表中。 (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Add](../../aspose.cells.vba/vbamodulecollection/add#add_1)(Worksheet) | 为工作表添加模块。 |
| [Add](../../aspose.cells.vba/vbamodulecollection/add#add)(VbaModuleType, string) | 添加模块。 |
| [AddDesignerStorage](../../aspose.cells.vba/vbamodulecollection/adddesignerstorage)(string, byte[]) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(VbaModule) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(VbaModule, IComparer&lt;VbaModule&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, VbaModule, IComparer&lt;VbaModule&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(VbaModule) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(VbaModule[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(VbaModule[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, VbaModule[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;VbaModule&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;VbaModule&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;VbaModule&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;VbaModule&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;VbaModule&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;VbaModule&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;VbaModule&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;VbaModule&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;VbaModule&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;VbaModule&gt;) |  |
| [GetDesignerStorage](../../aspose.cells.vba/vbamodulecollection/getdesignerstorage)(string) | 代表 Designer 的数据。 |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(VbaModule) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(VbaModule, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(VbaModule, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(VbaModule) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(VbaModule, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(VbaModule, int, int) |  |
| [Remove](../../aspose.cells.vba/vbamodulecollection/remove#remove_1)(string) | 按名称删除模块 |
| [Remove](../../aspose.cells.vba/vbamodulecollection/remove#remove)(Worksheet) | 删除工作表的模块。 |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### 例子

```csharp

[C#]

//实例化一个工作簿对象
Workbook workbook = new Workbook();
 // 初始化 VBA 项目。
VbaProject vbaProject = workbook.VbaProject; 
// 添加一个新模块。
vbaProject.Modules.Add(VbaModuleType.Class, "test");
//保存Excel文件
workbook.Save("book1.xlsm");

 [Visual Basic]

'实例化工作簿对象
Dim workbook As Workbook = New Workbook()
'初始化 VBA 项目。
Dim vbaProject as VbaProject  = workbook.VbaProject
'添加一个新模块。
vbaProject.Modules.Add(VbaModuleType.Class, "test")
'保存 Excel 文件
workbook.Save("book1.xlsm")
```

### 也可以看看

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [VbaModule](../vbamodule)
* 命名空间 [Aspose.Cells.Vba](../../aspose.cells.vba)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
