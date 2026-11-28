---
title: "Enum EquationNodeType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Equations.EquationNodeType enum. Denklem düğüm tipi. Not 1199 Şu anda kapsamda yalnızca bir düğüm var ve onun enum değeri 1'dir. Belirttiği düğüm matematik metni depolamak için kullanılır. 2100199 Düğümün bazı özel fonksiyon düğümlerinin bir bileşeni olduğunu gösterir. 3200 Düğümün bazı özel fonksiyonlara sahip olduğunu gösterir."
type: docs
url: /tr/net/aspose.cells.drawing.equations/equationnodetype/
---
## EquationNodeType enumeration

Denklem düğüm tipi. Not: (1)[1-99] Şu anda kapsamda yalnızca bir düğüm vardır ve onun numaralandırma değeri 1'dir. Belirttiği düğüm matematiksel metni depolamak için kullanılır. (2)[100-199] Düğümün bazı özel fonksiyon düğümlerinin bir bileşeni olduğunu gösterir. (3)[200-] Düğümün bazı özel işlevleri olduğunu gösterir.

```csharp
public enum EquationNodeType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| UnKnow | `0` | UnKnow |
| Text | `1` | matematik metni depolayan bir düğüm belirtir |
| Base | `100` | Bir Base bileşeni belirtir |
| Denominator | `101` | Bir Denominator bileşeni belirtir |
| Numerator | `102` | Bir Numerator bileşeni belirtir |
| FunctionName | `103` | Bir FunctionName bileşeni belirtir |
| Subscript | `104` | Bir Subscript bileşeni belirtir |
| Superscript | `105` | Bir Superscript bileşeni belirtir |
| Degree | `106` | Bir Degree bileşeni belirtir |
| MatrixRow | `107` | Bir MatrixRow bileşeni belirtir. Matrisin tek bir satırı |
| Limit | `108` | Lower-Limit işlevinin veya Upper-Limit işlevinin bir alt nesnesini temsil eder |
| EquationParagraph | `200` | Matematiksel bir paragrafı(oMathPara) belirtir. |
| MathematicalEquation | `201` | Bir denklem veya matematiksel ifadeyi(OMath) belirtir. |
| FractionEquation | `202` | Kesir denklemini belirtir |
| FunctionEquation | `203` | Fonksiyon denklemini belirtir |
| DelimiterEquation | `204` | Ayırıcı denklemini belirtir |
| NaryEquation | `205` | n-ary operatör denklemini belirtir |
| RadicalEquation | `206` | Kök denklemini belirtir |
| SuperscriptEquation | `207` | Üst simge denklemini belirtir |
| SubscriptEquation | `208` | Alt simge denklemini belirtir |
| SubSupEquation | `209` | İşlemlerin sağ tarafında üst ve alt simgeler bulunan bir denklemi belirtir. |
| PreSubSupEquation | `210` | İşlemlerin sol tarafında üst ve alt simgeler bulunan bir denklemi belirtir. |
| AccentEquation | `211` | Aksan denklemini belirtir |
| BarEquation | `212` | Bar denklemini belirtir |
| BorderBoxEquation | `213` | Kenarlık kutu denklemini belirtir |
| BoxEquation | `214` | Kutu denklemini belirtir |
| GroupCharacterEquation | `215` | Group-Character denklemini belirtir |
| MatrixEquation | `216` | Matrix denklemini belirtir, |
| LowerLimit | `217` | Lower-Limit fonksiyonunu belirtir |
| UpperLimit | `218` | Upper-Limit fonksiyonunu belirtir |
| Mathematical | `201` | Bir denklem veya matematiksel ifadeyi(OMath) belirtir. |
| Fraction | `202` | Kesir denklemini belirtir |
| Function | `203` | Fonksiyon denklemini belirtir |
| Delimiter | `204` | Ayırıcı denklemini belirtir |
| Nary | `205` | n-ary operatör denklemini belirtir |
| Radical | `206` | Kök denklemini belirtir |
| Sup | `207` | Üst simge denklemini belirtir |
| Sub | `208` | Alt simge denklemini belirtir |
| SubSup | `209` | İşlemlerin sağ tarafında üst ve alt simgeler bulunan bir denklemi belirtir. |
| PreSubSup | `210` | İşlemlerin sol tarafında üst ve alt simgeler bulunan bir denklemi belirtir. |
| Accent | `211` | Aksan denklemini belirtir |
| Bar | `212` | Bar denklemini belirtir |
| BorderBox | `213` | Kenarlık kutu denklemini belirtir |
| Box | `214` | Kutu denklemini belirtir |
| GroupChr | `215` | Group-Character denklemini belirtir |
| Matrix | `216` | Matrix denklemini belirtir, |
| ArrayEquation | `317` | Equation-Array fonksiyonunu belirtir. Fonksiyon bir veya daha fazla denklemeden oluşur. |

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına bir denklem ekle
            var equationShape = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Denklemin matematik düğümünü al
            EquationNode mathNode = equationShape.GetEquationParagraph().GetChild(0);

            // Circumflex karakteriyle bir aksan düğümü oluştur
            AccentEquationNode accentNode = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            accentNode.AccentCharacter = "\u0302";

            // Temel düğüm ve metin düğümünü ekle
            EquationNode baseNode = accentNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";

            // Çalışma kitabını kaydedin
            workbook.Save("EquationNodeTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


