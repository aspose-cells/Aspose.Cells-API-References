---
title: AddIdentify
second_title: Aspose.Cells for .NET API 参考
description: 设置每个页面字段中使用哪个项目标签来标识数据范围 pageItemIndex.Length必须等于PageFieldCount所以请先添加页面字段
type: docs
weight: 30
url: /zh/net/aspose.cells.pivot/pivotpagefields/addidentify/
---
## PivotPageFields.AddIdentify method

设置每个页面字段中使用哪个项目标签来标识数据范围。 pageItemIndex.Length必须等于PageFieldCount，所以请先添加页面字段。

```csharp
public void AddIdentify(int rangeIndex, int[] pageItemIndex)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| rangeIndex | Int32 | 合并数据范围索引。 |
| pageItemIndex | Int32[] | 每个页面字段中的页面项目索引。 pageItemIndex[2] = 1 表示第三个字段中的第二个项目用于标识此范围。 pageItemIndex[1] = -1 表示第二个字段中没有项目用于识别此范围 ，MS将在第二个字段中自动创建“空白”项目以识别此范围。 |

### 也可以看看

* class [PivotPageFields](../../pivotpagefields)
* 命名空间 [Aspose.Cells.Pivot](../../pivotpagefields)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
