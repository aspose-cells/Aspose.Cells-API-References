---
title: "MainWeb.OnShapeSelectedClientFunction"
second_title: "Справочник API Aspose.Cells для .NET"
description: "MainWeb свойство. Получает или задает клиентскую функцию, вызываемую при выборе фигуры. Клиентская функция должна быть объявлена следующим образом: function MyOnSelectShapeshape  var nameshape.getAttributenamevalue var textshape.getAttributetextvalue var valueshape.getAttributecontrolvalue var typeshape.getAttributemsotype. Примечание: вы можете использовать указатель this в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие."
type: docs
url: /ru/net/aspose.cells.gridweb/mainweb/onshapeselectedclientfunction/
---
## MainWeb.OnShapeSelectedClientFunction property

Получает или задает клиентскую функцию, которая будет вызываться при выборе фигуры. Клиентская функция должна быть объявлена так: function MyOnSelectShape(shape) { var name=shape.getAttribute(\"namevalue\") var text=shape.getAttribute(\"textvalue\") var value=shape.getAttribute(\"controlvalue\") var type=shape.getAttribute(\"msotype\") }Примечание: Вы можете использовать указатель \"this\" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие.

```csharp
public string OnShapeSelectedClientFunction { get; set; }
```

### См. также

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


