---
title: "Protection 类"
linktitle: "Protection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Protection 类。封装了在 Go 中表示 protection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/protection/
---

## Protection class

表示工作表可用的各种保护选项类型。

```go

type Protection struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [Copy](./copy/) | 复制保护信息。 |
| [GetAllowDeletingColumn](./getallowdeletingcolumn/) | 表示在受保护的工作表上是否允许删除列。 |
| [SetAllowDeletingColumn](./setallowdeletingcolumn/) | 表示在受保护的工作表上是否允许删除列。 |
| [GetAllowDeletingRow](./getallowdeletingrow/) | 表示在受保护的工作表上是否允许删除行。 |
| [SetAllowDeletingRow](./setallowdeletingrow/) | 表示在受保护的工作表上是否允许删除行。 |
| [GetAllowFiltering](./getallowfiltering/) | 表示用户是否被允许使用在工作表受保护之前创建的自动筛选。 |
| [SetAllowFiltering](./setallowfiltering/) | 表示用户是否被允许使用在工作表受保护之前创建的自动筛选。 |
| [GetAllowFormattingCell](./getallowformattingcell/) | 表示在受保护的工作表上是否允许对单元格进行格式设置。 |
| [SetAllowFormattingCell](./setallowformattingcell/) | 表示在受保护的工作表上是否允许对单元格进行格式设置。 |
| [GetAllowFormattingColumn](./getallowformattingcolumn/) | 表示在受保护的工作表上是否允许对列进行格式设置 |
| [SetAllowFormattingColumn](./setallowformattingcolumn/) | 表示在受保护的工作表上是否允许对列进行格式设置 |
| [GetAllowFormattingRow](./getallowformattingrow/) | 表示在受保护的工作表上是否允许对行进行格式设置 |
| [SetAllowFormattingRow](./setallowformattingrow/) | 表示在受保护的工作表上是否允许对行进行格式设置 |
| [GetAllowInsertingColumn](./getallowinsertingcolumn/) | 表示在受保护的工作表上是否允许插入列 |
| [SetAllowInsertingColumn](./setallowinsertingcolumn/) | 表示在受保护的工作表上是否允许插入列 |
| [GetAllowInsertingHyperlink](./getallowinsertinghyperlink/) | 表示在受保护的工作表上是否允许插入超链接 |
| [SetAllowInsertingHyperlink](./setallowinsertinghyperlink/) | 表示在受保护的工作表上是否允许插入超链接 |
| [GetAllowInsertingRow](./getallowinsertingrow/) | 表示在受保护的工作表上是否允许插入行 |
| [SetAllowInsertingRow](./setallowinsertingrow/) | 表示在受保护的工作表上是否允许插入行 |
| [GetAllowSorting](./getallowsorting/) | 表示在受保护的工作表上是否允许使用排序选项。 |
| [SetAllowSorting](./setallowsorting/) | 表示在受保护的工作表上是否允许使用排序选项。 |
| [GetAllowUsingPivotTable](./getallowusingpivottable/) | 表示用户是否被允许在受保护的工作表上操作透视表。 |
| [SetAllowUsingPivotTable](./setallowusingpivottable/) | 表示用户是否被允许在受保护的工作表上操作透视表。 |
| [GetAllowEditingContent](./getalloweditingcontent/) | 表示是否允许用户编辑受保护工作表中锁定单元格的内容。 |
| [SetAllowEditingContent](./setalloweditingcontent/) | 表示是否允许用户编辑受保护工作表中锁定单元格的内容。 |
| [GetAllowEditingObject](./getalloweditingobject/) | 表示是否允许用户在受保护工作表上操作绘图对象。 |
| [SetAllowEditingObject](./setalloweditingobject/) | 表示是否允许用户在受保护工作表上操作绘图对象。 |
| [GetAllowEditingScenario](./getalloweditingscenario/) | 表示是否允许用户编辑受保护工作表中的方案。 |
| [SetAllowEditingScenario](./setalloweditingscenario/) | 表示是否允许用户编辑受保护工作表中的方案。 |
| [GetAllowSelectingLockedCell](./getallowselectinglockedcell/) | 表示是否允许用户在受保护工作表中选择锁定的单元格。 |
| [SetAllowSelectingLockedCell](./setallowselectinglockedcell/) | 表示是否允许用户在受保护工作表中选择锁定的单元格。 |
| [GetAllowSelectingUnlockedCell](./getallowselectingunlockedcell/) | 表示是否允许用户在受保护工作表中选择未锁定的单元格。 |
| [SetAllowSelectingUnlockedCell](./setallowselectingunlockedcell/) | 表示是否允许用户在受保护工作表中选择未锁定的单元格。 |
| [GetPassword](./getpassword/) | 表示用于保护工作表的密码。 |
| [SetPassword](./setpassword/) | 表示用于保护工作表的密码。 |
| [IsProtectedWithPassword](./isprotectedwithpassword/) | 指示工作表是否已使用密码受保护。 |
| [VerifyPassword](./verifypassword/) | 验证密码。 |
| [GetPasswordHash](./getpasswordhash/) | 获取当前密码的哈希值。 |
