---
title: "Класс CellImage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridWeb.Data.CellImage. Представляет гиперссылку с изображением src"
type: docs
url: /ru/net/aspose.cells.gridweb.data/cellimage/
---
## CellImage class

Представляет гиперссылку с источником изображения.

```csharp
public class CellImage : Hyperlink
```

## Свойства

| Имя | Описание |
| --- | --- |
| virtual [ActionType](../../aspose.cells.gridweb.data/hyperlink/actiontype/) { get; set; } | Получает или задает тип действия гиперссылки. Он может быть ActionTpye.UrlLink или ActionType.CellCommand. Тип UrlLink означает, что гиперссылка ведёт на веб‑страницу или электронную почту. Например: "http://www.aspose.com" или "mailto:admin@aspose.com". Тип CellCommand означает, что гиперссылка вызовет событие CellCommand, и вы можете обработать это событие.(Inherited from [`Hyperlink`](../hyperlink/).) |
| [Area](../../aspose.cells.gridweb.data/hyperlink/area/) { get; } | Получает диапазон гиперссылки.(Inherited from [`Hyperlink`](../hyperlink/).) |
| [CellCommand](../../aspose.cells.gridweb.data/hyperlink/cellcommand/) { get; set; } | Получает или задает имя команды ячейки.(Inherited from [`Hyperlink`](../hyperlink/).) |
| virtual [DiscardInput](../../aspose.cells.gridweb.data/hyperlink/discardinput/) { get; set; } | Указывает, следует ли отбрасывать ввод пользователя в браузере клиента при щелчке по этой гиперссылке CellCommand. Может использоваться как действие "undo".(Inherited from [`Hyperlink`](../hyperlink/).) |
| virtual [ImageUrl](../../aspose.cells.gridweb.data/hyperlink/imageurl/) { get; set; } | Получает или задает URL изображения гиперссылки. Если установить null или пустую строку, гиперссылка будет отображать только свой текст.(Inherited from [`Hyperlink`](../hyperlink/).) |
| [Target](../../aspose.cells.gridweb.data/hyperlink/target/) { get; set; } | (Наследовано от [`Hyperlink`](../hyperlink/).) |
| virtual [Text](../../aspose.cells.gridweb.data/hyperlink/text/) { get; set; } | Получает или задает отображаемый текст гиперссылки.(Наследовано от [`Hyperlink`](../hyperlink/).) |
| virtual [ToolTip](../../aspose.cells.gridweb.data/hyperlink/tooltip/) { get; set; } | Получает или задает всплывающую подсказку гиперссылки.(Наследовано от [`Hyperlink`](../hyperlink/).) |
| virtual [Url](../../aspose.cells.gridweb.data/hyperlink/url/) { get; set; } | Получает или задает строку URL.(Наследовано от [`Hyperlink`](../hyperlink/).) |

### См. также

* class [Hyperlink](../hyperlink/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


