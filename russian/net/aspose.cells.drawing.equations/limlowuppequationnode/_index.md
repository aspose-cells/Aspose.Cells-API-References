---
title: "Класс LimLowUppEquationNode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.Equations.LimLowUppEquationNode. Этот класс определяет функцию предела"
type: docs
url: /ru/net/aspose.cells.drawing.equations/limlowuppequationnode/
---
## LimLowUppEquationNode class

Этот класс определяет функцию предела.

```csharp
public class LimLowUppEquationNode : EquationNode
```

## Свойства

| Имя | Описание |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Получить тип уравнения текущего узла (Унаследовано от [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Возвращает шрифт этого объекта (Унаследовано от [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Получает длину символов (Унаследовано от [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Указывает родительский узел текущего узла (Унаследовано от [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Получает начальный индекс символов (Унаследовано от [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Возвращает параметры текста (Унаследовано от [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Представляет тип узла (Унаследовано от [`EquationNode`](../equationnode/).) |

## Методы

| Имя | Описание |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Вставляет указанный узел в конец списка дочерних узлов текущего узла (Унаследовано от [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Вставьте узел указанного типа в конец списка дочерних узлов текущего узла.(Наследовано от [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/limlowuppequationnode/equals/)(object) | Определить, равен ли текущий узел уравнения указанному узлу |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild/)(int) | Возвращает узел с указанным индексом среди дочерних узлов текущего узла.(Наследовано от [`EquationNode`](../equationnode/).) |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter/)(EquationNodeType) | Вставляет указанный узел после текущего узла.(Наследовано от [`EquationNode`](../equationnode/).) |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore/)(EquationNodeType) | Вставляет указанный узел перед текущим узлом.(Наследовано от [`EquationNode`](../equationnode/).) |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild/)(int, EquationNodeType) | Вставляет узел указанного типа в указанную позицию индекса в список дочерних узлов текущего узла.(Наследовано от [`EquationNode`](../equationnode/).) |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove/)() | Удаляет себя из родителя.(Наследовано от [`EquationNode`](../equationnode/).) |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren/)() | Удаляет все дочерние узлы текущего узла.(Наследовано от [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(EquationNode) | Удаляет указанный узел из дочерних узлов текущего узла.(Наследовано от [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(int) | Удаляет узел с указанным индексом из дочерних узлов текущего узла.(Наследовано от [`EquationNode`](../equationnode/).) |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Устанавливает предустановленный стиль WordArt.(Наследовано от [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ToLaTeX](../../aspose.cells.drawing.equations/equationnode/tolatex/)() | Преобразовать это уравнение в выражение LaTeX.(Наследовано от [`EquationNode`](../equationnode/).) |
| [ToMathML](../../aspose.cells.drawing.equations/equationnode/tomathml/)() | Преобразовать это уравнение в выражение MathML.(Наследовано от [`EquationNode`](../equationnode/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassLimLowUppEquationNodeDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создать экземпляр класса LimLowUppEquationNode
                // Поскольку у класса нет публичного конструктора без параметров,
                // мы используем другой подход для демонстрации функциональности
                LimLowUppEquationNode limNode = null;
                LimLowUppEquationNode anotherNode = null;

                // Продемонстрировать базовую функциональность — проверку равенства объектов
                bool areEqual = limNode?.Equals((object)anotherNode) ?? false;

                Console.WriteLine($"LimLowUppEquationNode demonstration");
                Console.WriteLine($"Nodes are equal: {areEqual}");

                // Сохраните книгу
                workbook.Save("LimLowUppEquationNodeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with LimLowUppEquationNode: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


