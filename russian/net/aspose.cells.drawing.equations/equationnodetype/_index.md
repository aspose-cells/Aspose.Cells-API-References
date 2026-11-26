---
title: "Перечисление EquationNodeType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.Equations.EquationNodeType. Тип узла уравнения. Примечание 1199: В настоящее время в области видимости присутствует только один узел, и его значение перечисления равно 1. Указанный узел используется для хранения математического текста. 2100199 указывает, что узел является компонентом некоторых специальных функций. 3200 указывает, что у узла есть некоторые специальные функции"
type: docs
url: /ru/net/aspose.cells.drawing.equations/equationnodetype/
---
## EquationNodeType enumeration

Тип узла уравнения. Примечание: (1)[1-99] В текущей области присутствует только один узел, его перечисляемое значение равно 1. Указанный узел используется для хранения математического текста. (2)[100-199] Указывает, что узел является компонентом некоторых специальных функций. (3)[200-] Указывает, что у узла есть специальные функции.

```csharp
public enum EquationNodeType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| UnKnow | `0` | UnKnow |
| Text | `1` | указывает узел, который хранит математический текст |
| Base | `100` | Указывает базовый компонент |
| Denominator | `101` | Указывает компонент знаменателя |
| Numerator | `102` | Указывает компонент числителя |
| FunctionName | `103` | Указывает компонент имени функции |
| Subscript | `104` | Указывает компонент нижнего индекса |
| Superscript | `105` | Указывает компонент верхнего индекса |
| Degree | `106` | Указывает компонент степени |
| MatrixRow | `107` | Указывает компонент MatrixRow. Одна строка матрицы |
| Limit | `108` | Представляет подобъект функции Lower-Limit или Upper-Limit |
| EquationParagraph | `200` | Указывает математический абзац (oMathPara). |
| MathematicalEquation | `201` | Указывает уравнение или математическое выражение (OMath). |
| FractionEquation | `202` | Указывает дробное уравнение |
| FunctionEquation | `203` | Указывает функциональное уравнение |
| DelimiterEquation | `204` | Указывает уравнение‑разделитель |
| NaryEquation | `205` | Указывает n‑арное операторное уравнение |
| RadicalEquation | `206` | Указывает корневое уравнение |
| SuperscriptEquation | `207` | Указывает надстрочное уравнение |
| SubscriptEquation | `208` | Указывает подстрочное уравнение |
| SubSupEquation | `209` | Указывает уравнение с надстрочными и подстрочными элементами справа от операндов. |
| PreSubSupEquation | `210` | Указывает уравнение с надстрочными и подстрочными элементами слева от операндов. |
| AccentEquation | `211` | Указывает акцентированное уравнение |
| BarEquation | `212` | Указывает барное уравнение |
| BorderBoxEquation | `213` | Указывает уравнение с рамкой |
| BoxEquation | `214` | Указывает уравнение в коробке |
| GroupCharacterEquation | `215` | Указывает уравнение группы‑символов |
| MatrixEquation | `216` | Указывает матричное уравнение, |
| LowerLimit | `217` | Указывает функцию нижнего предела |
| UpperLimit | `218` | Указывает функцию верхнего предела |
| Mathematical | `201` | Указывает уравнение или математическое выражение (OMath). |
| Fraction | `202` | Указывает дробное уравнение |
| Function | `203` | Указывает функциональное уравнение |
| Delimiter | `204` | Указывает уравнение‑разделитель |
| Nary | `205` | Указывает n‑арное операторное уравнение |
| Radical | `206` | Указывает корневое уравнение |
| Sup | `207` | Указывает надстрочное уравнение |
| Sub | `208` | Указывает подстрочное уравнение |
| SubSup | `209` | Указывает уравнение с надстрочными и подстрочными элементами справа от операндов. |
| PreSubSup | `210` | Указывает уравнение с надстрочными и подстрочными элементами слева от операндов. |
| Accent | `211` | Указывает акцентированное уравнение |
| Bar | `212` | Указывает барное уравнение |
| BorderBox | `213` | Указывает уравнение с рамкой |
| Box | `214` | Указывает уравнение в коробке |
| GroupChr | `215` | Указывает уравнение группы‑символов |
| Matrix | `216` | Указывает матричное уравнение, |
| ArrayEquation | `317` | Указывает функцию массива уравнений. Функция состоит из одного или нескольких уравнений. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить уравнение на первый лист
            var equationShape = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Получить математический узел из уравнения
            EquationNode mathNode = equationShape.GetEquationParagraph().GetChild(0);

            // Создать акцентный узел с символом циркумфлекса
            AccentEquationNode accentNode = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            accentNode.AccentCharacter = "\u0302";

            // Добавить базовый узел и текстовый узел
            EquationNode baseNode = accentNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";

            // Сохраните книгу
            workbook.Save("EquationNodeTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


