---
title: "Sınıf CustomCommandButton"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridWeb.CustomCommandButton sınıfı. GridWeb denetiminin sekme çubuğunda özel bir komut düğmesini temsil eder."
type: docs
url: /tr/net/aspose.cells.gridweb/customcommandbutton/
---
## CustomCommandButton class

GridWeb kontrolünün sekme çubuğunda özel bir komut düğmesini temsil eder.

```csharp
public class CustomCommandButton : Control, ISerializable
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [CustomCommandButton](customcommandbutton/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ClientClickEvent](../../aspose.cells.gridweb/customcommandbutton/clientclickevent/) { get; set; } | İstemci tarafında tıklama olayı işleyicisini alır veya ayarlar. |
| [Command](../../aspose.cells.gridweb/customcommandbutton/command/) { get; set; } | Komut adını alır veya ayarlar. |
| [CommandType](../../aspose.cells.gridweb/customcommandbutton/commandtype/) { get; set; } | Komutun renderleme türünü alır veya ayarlar. Tür, komut düğmesi veya bağlam menüsü öğesi olabilir. |
| [DiscardInput](../../aspose.cells.gridweb/customcommandbutton/discardinput/) { get; set; } | Kullanıcı bu düğmeye tıkladığında istemci tarayıcısındaki kullanıcı girdisinin atılıp atılmayacağını gösterir. "Geri al" eylemi olarak kullanılabilir. |
| [ImageUrl](../../aspose.cells.gridweb/customcommandbutton/imageurl/) { get; set; } | Komut düğmesinin görüntü URL'sini alır veya ayarlar. Null veya boş dizeye ayarlanırsa, düğme yalnızca metnini gösterir. |
| [Text](../../aspose.cells.gridweb/customcommandbutton/text/) { get; set; } | Komut düğmesinin alternatif metnini alır veya ayarlar. |
| [ToolTip](../../aspose.cells.gridweb/customcommandbutton/tooltip/) { get; set; } | Komut düğmesinin araç ipucunu alır veya ayarlar. |
| [Width](../../aspose.cells.gridweb/customcommandbutton/width/) { get; set; } | Düğmenin genişliği. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetObjectData](../../aspose.cells.gridweb/customcommandbutton/getobjectdata/)(SerializationInfo, StreamingContext) | Sadece dahili kullanım için. |

### Örnekler

```csharp
[C#]
GridWebBean GridWeb1=ExtPage.getInstance().getBean();
CustomCommandButton button = new CustomCommandButton();
button.Command = "MyCommand";
button.ImageUrl = "images/button1.gif";
GridWeb1.CustomCommandButtons.Add(button);
[VB]
Dim button As CustomCommandButton =  New CustomCommandButton()
button.Command = "MyCommand"
button.ImageUrl = "images/button1.gif"
GridWeb1.CustomCommandButtons.Add(button)
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


