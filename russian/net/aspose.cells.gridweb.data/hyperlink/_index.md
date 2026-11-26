---
title: "Класс Hyperlink"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.GridWeb.Data.Hyperlink класс."
type: docs
url: /ru/net/aspose.cells.gridweb.data/hyperlink/
---
## Hyperlink class

```csharp
[Obsolete("This class is obsolete; use GridHyperlink instead")]
public class Hyperlink
```

## Свойства

| Имя | Описание |
| --- | --- |
| virtual [ActionType](../../aspose.cells.gridweb.data/hyperlink/actiontype/) { get; set; } | Получает или задаёт тип действия гиперссылки. Он может быть ActionTpye.UrlLink или ActionType.CellCommand. Тип UrlLink означает, что гиперссылка указывает на веб‑страницу или электронную почту. Например: "http://www.aspose.com" или "mailto:admin@aspose.com". Тип CellCommand означает, что гиперссылка вызовет событие CellCommand, которое вы можете обработать. |
| [Area](../../aspose.cells.gridweb.data/hyperlink/area/) { get; } | Получает диапазон гиперссылки. |
| [CellCommand](../../aspose.cells.gridweb.data/hyperlink/cellcommand/) { get; set; } | Получает или задаёт имя команды ячейки. |
| virtual [DiscardInput](../../aspose.cells.gridweb.data/hyperlink/discardinput/) { get; set; } | Указывает, следует ли отбрасывать ввод пользователя в браузере клиента при щелчке по этой гиперссылке CellCommand. Может использоваться как действие "undo". |
| virtual [ImageUrl](../../aspose.cells.gridweb.data/hyperlink/imageurl/) { get; set; } | Получает или задаёт URL изображения гиперссылки. Если установить значение null или пустую строку, гиперссылка будет отображать только свой текст. |
| [Target](../../aspose.cells.gridweb.data/hyperlink/target/) { get; set; } |  |
| virtual [Text](../../aspose.cells.gridweb.data/hyperlink/text/) { get; set; } | Получает или задаёт отображаемый текст гиперссылки. |
| virtual [ToolTip](../../aspose.cells.gridweb.data/hyperlink/tooltip/) { get; set; } | Получает или задаёт всплывающую подсказку гиперссылки. |
| virtual [Url](../../aspose.cells.gridweb.data/hyperlink/url/) { get; set; } | Получает или задаёт строку URL. |

### См. также

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


