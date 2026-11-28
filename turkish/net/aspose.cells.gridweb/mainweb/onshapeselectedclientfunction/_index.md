---
title: "MainWeb.OnShapeSelectedClientFunction"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MainWeb özelliği. Bir şekil seçildiğinde çağrılacak istemci tarafı işlevi alır veya ayarlar. İstemci işlevi aşağıdaki gibi tanımlanmalıdır: function MyOnSelectShapeshape  var nameshape.getAttributenamevalue var textshape.getAttributetextvalue var valueshape.getAttributecontrolvalue var typeshape.getAttributemsotype  Not: Bu işlevde this işaretçisini, olayı tetikleyen grid kontrolüne işaret etmek için kullanabilirsiniz"
type: docs
url: /tr/net/aspose.cells.gridweb/mainweb/onshapeselectedclientfunction/
---
## MainWeb.OnShapeSelectedClientFunction property

Bir şekil seçildiğinde çağrılacak istemci tarafı işlevi alır veya ayarlar. İstemci işlevi şu şekilde tanımlanmalıdır: function MyOnSelectShape(shape) { var name=shape.getAttribute("namevalue") var text=shape.getAttribute("textvalue") var value=shape.getAttribute("controlvalue") var type=shape.getAttribute("msotype") }Not: İstemci işlevinde "this" işaretçisini, olayı tetikleyen ızgara kontrolüne işaret etmek için kullanabilirsiniz.

```csharp
public string OnShapeSelectedClientFunction { get; set; }
```

### Ayrıca Bakınız

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


