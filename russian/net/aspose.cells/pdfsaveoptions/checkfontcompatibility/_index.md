---
title: CheckFontCompatibility
second_title: Справочник по Aspose.Cells для .NET API
description: Указывает следует ли проверять совместимость шрифтов для каждого символа в тексте.
type: docs
weight: 50
url: /ru/net/aspose.cells/pdfsaveoptions/checkfontcompatibility/
---
## PdfSaveOptions.CheckFontCompatibility property

Указывает, следует ли проверять совместимость шрифтов для каждого символа в тексте.

```csharp
public bool CheckFontCompatibility { get; set; }
```

### Примечания

Значение по умолчанию — true. Отключение этого свойства может повысить производительность. Но если для его отображения нельзя использовать заданный по умолчанию или указанный шрифт текста/символов, в сгенерированном PDF-файле могут появиться нечитаемые символы (например, блоки). В такой ситуации пользователь должен оставить это свойство равным true, чтобы можно было найти альтернативный шрифт и использовать его для отображения текста;

### Смотрите также

* class [PdfSaveOptions](../../pdfsaveoptions)
* пространство имен [Aspose.Cells](../../pdfsaveoptions)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
