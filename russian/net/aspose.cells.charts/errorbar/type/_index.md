---
title: Type
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет тип суммы полосы ошибок.
type: docs
weight: 60
url: /ru/net/aspose.cells.charts/errorbar/type/
---
## ErrorBar.Type property

Представляет тип суммы полосы ошибок.

```csharp
public ErrorBarType Type { get; set; }
```

### Примеры

```csharp
[C#]
//Устанавливает пользовательский тип полосы ошибок
aseries.YErrorBar.Type = ErrorBarType.InnerCustom;
aseries.YErrorBar.PlusValue = "=Sheet1!A1";
aseries.YErrorBar.MinusValue = "=Sheet1!A2";

[Visual Basic]
'Устанавливает пользовательский тип полосы ошибок
aseries.YErrorBar.Type = ErrorBarType.InnerCustom
aseries.YErrorBar.PlusValue = "=Sheet1!A1"
aseries.YErrorBar.MinusValue = "=Sheet1!A2"
```

### Смотрите также

* enum [ErrorBarType](../../errorbartype)
* class [ErrorBar](../../errorbar)
* пространство имен [Aspose.Cells.Charts](../../errorbar)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
