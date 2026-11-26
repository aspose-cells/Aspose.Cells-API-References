---
title: "Перечисление EquationCombiningCharacterType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.Equations.EquationCombiningCharacterType. Тип комбинирующих символов"
type: docs
url: /ru/net/aspose.cells.drawing.equations/equationcombiningcharactertype/
---
## EquationCombiningCharacterType enumeration

Тип комбинирующих символов.

```csharp
public enum EquationCombiningCharacterType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Unknown | `-1` | Используйте тип unknown, когда он не найден в существующем типе. |
| DotAbove | `0` | "̇" Unicode: u0307 Комбинирующая точка сверху |
| Diaeresis | `1` | "̈" Unicode: u0308 Комбинирующая диарезис |
| ThreeDotsAbove | `2` | "⃛" Unicode: u20db Комбинирующие три точки сверху |
| CircumflexAccent | `3` | "̂" Unicode: u0302 Комбинирующий циркумфлекс |
| Caron | `4` | "̌" Unicode: u030c Комбинирующий карон |
| AcuteAccent | `5` | "́" Unicode: u0301 Комбинирующий острый акцент |
| GraveAccent | `6` | "̀" Unicode: u0300 Комбинирующий гравис |
| Breve | `7` | "̆" Unicode: u0306 Комбинирующий бреве |
| Tilde | `8` | "̃" Unicode: u0303 Комбинирующая тильда |
| Overline | `9` | "̅" Unicode: u0305 Комбинирующее надчеркивание |
| DoubleOverline | `10` | "̿" Unicode: u033f Комбинирующее двойное надчеркивание |
| TopCurlyBracket | `11` | "⏞" Unicode: u23de Комбинирующая верхняя фигурная скобка |
| BottomCurlyBracket | `12` | "⏟" Unicode: u23df Комбинирующая нижняя фигурная скобка |
| LeftArrowAbove | `13` | "⃖" Unicode: u20d6 Комбинирующая левая стрелка сверху |
| RightArrowAbove | `14` | "⃗" Unicode: u20d7 Комбинирующая правая стрелка сверху |
| LeftRightArrowAbove | `15` | "⃡" Unicode: u20e1 Комбинирующая стрелка влево-вправо сверху |
| LeftHarpoonAbove | `16` | "⃐" Unicode: u20d0 Комбинирующая левая гарпун сверху |
| RightHarpoonAbove | `17` | "⃑" Unicode: u20d1 Комбинирующая правая гарпун сверху |
| LeftwardsArrow | `18` | "←" Unicode: u2190 Стрелка влево |
| RightwardsArrow | `19` | "→" Unicode: u2192 Стрелка вправо |
| LeftRightArrow | `20` | "↔" Unicode: u2194 Стрелка влево-вправо |
| LeftwardsDoubleArrow | `21` | "⇐" Unicode: u21d0 Двойная стрелка влево |
| RightwardsDoubleArrow | `22` | "⇒" Unicode: u21d2 Двойная стрелка вправо |
| LeftRightDoubleArrow | `23` | "⇔" Unicode: u21d4 Двойная стрелка влево-вправо |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationCombiningCharacterTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            GroupCharacterEquationNode node = (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            node.Position = EquationCharacterPositionType.Top;
            node.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            EquationNode subBase = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode textRun = (TextRunEquationNode)(subBase.AddChild(EquationNodeType.Text));
            textRun.Text = "abc";

            string resultFile = "GroupCharacterEquationTest.xlsx";
            workbook.Save(resultFile);

            // Проверьте сохранённый файл
            Workbook workbook2 = new Workbook(resultFile);
            TextBox textBoxRead = (TextBox)workbook2.Worksheets[0].Shapes[0];
            EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
            GroupCharacterEquationNode node2 = (GroupCharacterEquationNode)mathNode2.GetChild(0);

            Console.WriteLine("Equation Type: " + node2.EquationType);
            Console.WriteLine("Position: " + node2.Position);
            Console.WriteLine("Character Type: " + node2.ChrType);
            Console.WriteLine("Group Character: " + node2.GroupChr);

            EquationNode baseNode = node2.GetChild(0);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.GetChild(0);
            Console.WriteLine("Text Content: " + textNode.Text);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


