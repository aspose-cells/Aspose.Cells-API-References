---
title: "MainWeb.OnContextMenuShowClientFunction"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MainWeb özelliği. Bağlam menüsü gösterildiğinde çağrılacak istemci tarafı işlevi alır veya ayarlar. İstemci işlevi şu şekilde tanımlanmalıdır: function onContextMenuShow  var menu  event.srcElement menu.setItemVisibilityDelete block menu.setItemVisibilityUpdate none Not: Olayı tetikleyen ızgara kontrolunu işaret etmek için istemci işlevinde this işaretçisini kullanabilirsiniz"
type: docs
url: /tr/net/aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction/
---
## MainWeb.OnContextMenuShowClientFunction property

İçerik menüsü gösterildiğinde çağrılacak istemci tarafı işlevi alır veya ayarlar. İstemci işlevi şu şekilde tanımlanmalıdır: function onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility("Delete", "block"); menu.setItemVisibility("Update", "none"); }Not: İstemci işlevinde "this" işaretçisini, olayı tetikleyen ızgara kontrolüne işaret etmek için kullanabilirsiniz.

```csharp
public string OnContextMenuShowClientFunction { get; set; }
```

### Ayrıca Bakınız

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


