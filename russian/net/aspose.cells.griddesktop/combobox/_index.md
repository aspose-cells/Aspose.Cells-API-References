---
title: "Класс ComboBox"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridDesktop.ComboBox. Представляет элемент управления комбобоксом ячейки"
type: docs
url: /ru/net/aspose.cells.griddesktop/combobox/
---
## ComboBox class

Представляет элемент управления комбобоксом в ячейке.

```csharp
public class ComboBox : CellControl
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Height](../../aspose.cells.griddesktop/combobox/height/) { get; set; } | Получает или задает высоту элемента управления списком. |
| [IsInputable](../../aspose.cells.griddesktop/combobox/isinputable/) { get; set; } | Указывает, может ли пользователь вводить текст в комбобокс. Введённый текст будет сохранён как значение ячейки. Значение по умолчанию — "false". |
| [Items](../../aspose.cells.griddesktop/combobox/items/) { get; } | Получает объект, представляющий коллекцию элементов, содержащихся в этом ComboBox. |
| [SelectedIndex](../../aspose.cells.griddesktop/combobox/selectedindex/) { get; set; } | Получает или задает индекс, указывающий текущий выбранный элемент. При установке индекса будет автоматически вызываться метод GridDesktop.RunAllFormulas, если свойство GridDesktop.RecalculateFormulas равно true. |
| [Text](../../aspose.cells.griddesktop/cellcontrol/text/) { get; set; } | Получает или задает текст, связанный с этим элементом управления.(Унаследовано от [`CellControl`](../cellcontrol/).) |
| [Values](../../aspose.cells.griddesktop/combobox/values/) { get; } | Получает объект, представляющий коллекцию значений, содержащихся в этом ComboBox. |
| [Width](../../aspose.cells.griddesktop/combobox/width/) { get; set; } | Получает или задает ширину элемента управления списком. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetSelectedIndex](../../aspose.cells.griddesktop/combobox/setselectedindex/)(int) | Устанавливает выбранный индекс ComboBox. Это не вычислит формулу. Чтобы вычислить формулу, необходимо вызвать GridDesktop.RunAllFormulas вручную. Формулы не будут вычисляться автоматически ни при каких обстоятельствах, даже если GridDesktop.RecalculateFormulas равно true. |

### См. также

* class [CellControl](../cellcontrol/)
* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


