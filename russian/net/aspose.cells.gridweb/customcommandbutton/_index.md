---
title: "Класс CustomCommandButton"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridWeb.CustomCommandButton. Представляет пользовательскую кнопку команды на панели вкладок управления GridWeb."
type: docs
url: /ru/net/aspose.cells.gridweb/customcommandbutton/
---
## CustomCommandButton class

Представляет пользовательскую кнопку команды в панели вкладок управления GridWeb.

```csharp
public class CustomCommandButton : Control, ISerializable
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [CustomCommandButton](customcommandbutton/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [ClientClickEvent](../../aspose.cells.gridweb/customcommandbutton/clientclickevent/) { get; set; } | Получает или задаёт обработчик события щелчка на клиентской стороне. |
| [Command](../../aspose.cells.gridweb/customcommandbutton/command/) { get; set; } | Получает или задаёт имя команды. |
| [CommandType](../../aspose.cells.gridweb/customcommandbutton/commandtype/) { get; set; } | Получает или задаёт тип отображения команды. Тип может быть кнопкой команды или элементом контекстного меню. |
| [DiscardInput](../../aspose.cells.gridweb/customcommandbutton/discardinput/) { get; set; } | Указывает, следует ли отбрасывать ввод пользователя в браузере клиента, когда пользователь нажимает эту кнопку. Может использоваться как действие «отмена». |
| [ImageUrl](../../aspose.cells.gridweb/customcommandbutton/imageurl/) { get; set; } | Получает или задаёт URL изображения кнопки команды. Если установить null или пустую строку, кнопка будет отображать только свой текст. |
| [Text](../../aspose.cells.gridweb/customcommandbutton/text/) { get; set; } | Получает или задаёт альтернативный текст кнопки команды. |
| [ToolTip](../../aspose.cells.gridweb/customcommandbutton/tooltip/) { get; set; } | Получает или задаёт всплывающую подсказку кнопки команды. |
| [Width](../../aspose.cells.gridweb/customcommandbutton/width/) { get; set; } | Ширина кнопки. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetObjectData](../../aspose.cells.gridweb/customcommandbutton/getobjectdata/)(SerializationInfo, StreamingContext) | Используется только внутри. |

### Примеры

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

### См. также

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


