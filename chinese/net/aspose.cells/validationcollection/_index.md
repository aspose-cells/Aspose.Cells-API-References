---
title: ValidationCollection
second_title: Aspose.Cells for .NET API 参考
description: 表示数据验证集合
type: docs
weight: 6220
url: /zh/net/aspose.cells/validationcollection/
---
## ValidationCollection class

表示数据验证集合。

```csharp
public class ValidationCollection : CollectionBase<Validation>
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/validationcollection/item) { get; } | 获取[`Validation`](../validation)指定索引处的元素。 |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Add](../../aspose.cells/validationcollection/add#add_1)(CellArea) | 向集合添加数据验证。 |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Validation) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Validation, IComparer&lt;Validation&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Validation, IComparer&lt;Validation&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Validation) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Validation[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Validation[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Validation[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Validation&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Validation&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Validation&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Validation&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Validation&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Validation&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Validation&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Validation&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Validation&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Validation&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [GetValidationInCell](../../aspose.cells/validationcollection/getvalidationincell)(int, int) | 获取应用于给定单元格的验证。 |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Validation) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Validation, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Validation, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Validation) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Validation, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Validation, int, int) |  |
| [RemoveACell](../../aspose.cells/validationcollection/removeacell)(int, int) | 删除单元格上的所有验证设置。 |
| [RemoveArea](../../aspose.cells/validationcollection/removearea)(CellArea) | 删除范围内的所有验证设置.. |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### 例子

```csharp
[C#]
Workbook workbook = new Workbook();
ValidationCollection validations = workbook.Worksheets[0].Validations;
CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
Validation validation = validations[validations.Add(area)];
validation.Type = Aspose.Cells.ValidationType.List;
validation.Formula1 = "a,b,c,d";

[Visual Basic]
Dim workbook as Workbook = new Workbook()
Dim validations as ValidationCollection  = workbook.Worksheets(0).Validations
Dim area as CellArea = CellArea.CreateCellArea(0, 0, 1, 1);
Dim validation as Validation = validations(validations.Add(area))
validation.Type = ValidationType.List
validation.Formula1 = "a,b,c,d";
```

### 也可以看看

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Validation](../validation)
* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
