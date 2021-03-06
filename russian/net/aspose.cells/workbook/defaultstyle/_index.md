---
title: DefaultStyle
second_title: Справочник по Aspose.Cells для .NET API
description: Получает или задает объект по умолчаниюStyleaspose.cells/styleрабочей книги.
type: docs
weight: 130
url: /ru/net/aspose.cells/workbook/defaultstyle/
---
## Workbook.DefaultStyle property

Получает или задает объект по умолчанию[`Style`](../../style)рабочей книги.

```csharp
public Style DefaultStyle { get; set; }
```

### Примечания

Свойство DefaultStyle полезно для реализации стиля для всей книги.

### Примеры

Следующий код создает и создает новую рабочую книгу и устанавливает значение по умолчанию[`Style`](../../style)к нему.

```csharp
[C#]
Workbook workbook = new Workbook();
Style defaultStyle = workbook.DefaultStyle;
defaultStyle.Font.Name = "Tahoma";
workbook.DefaultStyle = defaultStyle;

[Visual Basic]
Dim workbook as Workbook = new Workbook()
Dim defaultStyle as Style = workbook.DefaultStyle
defaultStyle.Font.Name = "Tahoma"
workbook.DefaultStyle = defaultStyle
```

### Смотрите также

* class [Style](../../style)
* class [Workbook](../../workbook)
* пространство имен [Aspose.Cells](../../workbook)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
