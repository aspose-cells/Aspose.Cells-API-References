---
title: "GridJsWorkbook.InsertImage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridJsWorkbook. Вставляет изображение в лист из файлового потока или URL; должен быть предоставлен либо файловый поток, либо URL; либо вставляет форму, когда p.type является одним из AutoShapeType"
type: docs
url: /ru/net/aspose.cells.gridjs/gridjsworkbook/insertimage/
---
## GridJsWorkbook.InsertImage method

Вставляет изображение в лист из потока файла или URL (необходимо предоставить либо поток файла, либо URL) или вставляет форму, когда p.type является одним из AutoShapeType

```csharp
public string InsertImage(string uid, string p, Stream s, string imageUrl)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | String | Уникальный идентификатор для кеша файлов |
| p | String | Строка формата JSON для операции, указывающей расположение ячейки, имя листа, номер верхней левой строки, номер верхнего левого столбца для изображения и т.д. {name:'sheet1',ri:1,ci:1} |
| s | Stream | Файловый поток файла изображения |
| imageUrl | String | URL файла изображения |

### Возвращаемое значение

Строка формата JSON вставленного изображения

### См. также

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


