---
title: "AbstractFormulaChangeMonitor 类"
linktitle: "AbstractFormulaChangeMonitor"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "AbstractFormulaChangeMonitor 类。封装在 Go 中表示 abstractformulachangemonitor 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/abstractformulachangemonitor/
---

## AbstractFormulaChangeMonitor class

监视用户在特定操作期间跟踪公式的更改。

```go

type AbstractFormulaChangeMonitor struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [OnCellFormulaChanged](./oncellformulachanged/) | 当单元格中的公式更改时将触发的事件。 |
| [OnFormatConditionFormulaChanged](./onformatconditionformulachanged/) | 当 FormatCondition 的公式更改时将触发的事件。 |
