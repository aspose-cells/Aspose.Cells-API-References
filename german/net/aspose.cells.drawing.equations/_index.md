---
title: "Aspose.Cells.Drawing.Equations"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Der Aspose.Cells.Drawing.Equations Namespace bietet Klassen zum Erstellen verschiedener Gleichungsformen wie Bruchgleichungen, Potenzgleichungen usw. über Gleichungsknoten."
type: docs
url: /de/net/aspose.cells.drawing.equations/
---
Der **Aspose.Cells.Drawing.Equations** Namespace stellt Klassen zum Erstellen verschiedener Gleichungsformen (wie Bruchgleichungen, Potenzgleichungen usw.) über Gleichungsknoten bereit.

## Klassen

| Klasse | Beschreibung |
| --- | --- |
| [AccentEquationNode](./accentequationnode/) | Diese Klasse definiert eine Akzentgleichung, bestehend aus einer Basiskomponente und einem kombinierenden Diakritikum. |
| [ArrayEquationNode](./arrayequationnode/) | Definiert die Equation-Array-Funktion, ein Objekt, das aus einer oder mehreren Gleichungen besteht. |
| [BarEquationNode](./barequationnode/) | Diese Klasse definiert die Balkengleichung, bestehend aus einem Basisargument und einem Über‑ oder Unterstrich. |
| [BorderBoxEquationNode](./borderboxequationnode/) | Diese Klasse definiert die Border‑Box-Funktion, bestehend aus einem um eine Gleichung gezeichneten Rahmen. |
| [BoxEquationNode](./boxequationnode/) | Diese Klasse definiert die Box‑Funktion, die zum Gruppieren von Komponenten einer Gleichung verwendet wird. |
| [DelimiterEquationNode](./delimiterequationnode/) | Diese Klasse definiert die Trennzeichen‑Gleichung, bestehend aus öffnenden und schließenden Trennzeichen (wie Klammern, geschweiften Klammern, eckigen Klammern und senkrechten Strichen) sowie einer darin enthaltenen Komponente. Das Trennzeichen kann mehr als eine Komponente haben, wobei ein festgelegtes Trennzeichen zwischen den Komponenten steht. |
| [EquationComponentNode](./equationcomponentnode/) | Diese Klasse definiert die Komponenten einer Gleichung oder mathematischen Ausdrucks. Verschiedene Komponententypen werden zu unterschiedlichen Gleichungen kombiniert. Zum Beispiel besteht ein Bruch aus zwei Teilen, einer Zähler‑Komponente und einer Nenner‑Komponente. Für weitere Komponententypen siehe bitte 'EquationNodeType'. |
| [EquationNode](./equationnode/) | Abstrakte Klasse zum Ableiten anderer Gleichungsknoten. |
| [EquationNodeParagraph](./equationnodeparagraph/) | Diese Klasse definiert einen mathematischen Absatz, der ein oder mehrere MathEquationNode(OMath)-Elemente enthält. |
| [FractionEquationNode](./fractionequationnode/) | Diese Klasse definiert die Bruchgleichung, bestehend aus einem Zähler und einem Nenner, getrennt durch einen Bruchstrich. Der Bruchstrich kann horizontal oder diagonal sein, abhängig von den Bruch‑Eigenschaften. Die Bruchgleichung wird auch verwendet, um die Stapel‑Funktion darzustellen, bei der ein Element über einem anderen platziert wird, ohne Bruchstrich. |
| [FunctionEquationNode](./functionequationnode/) | Diese Klasse spezifiziert die Function-Apply-Gleichung, die aus einem Funktionsnamen und einem darauf angewendeten Argument besteht. Die Typen der Namens‑ und Argumentkomponenten sind jeweils 'EquationNodeType.FunctionName' und 'EquationNodeType.Base'. |
| [GroupCharacterEquationNode](./groupcharacterequationnode/) | Diese Klasse spezifiziert die Group-Character‑Funktion, die aus einem über oder unter dem Text gezeichneten Zeichen besteht, häufig mit dem Zweck, Elemente visuell zu gruppieren. |
| [LimLowUppEquationNode](./limlowuppequationnode/) | Diese Klasse spezifiziert die Grenzwert‑Funktion. |
| [MathematicalEquationNode](./mathematicalequationnode/) | Diese Klasse spezifiziert eine Gleichung oder einen mathematischen Ausdruck. Alle mathematischen Texte von Gleichungen oder mathematischen Ausdrücken werden von dieser Klasse enthalten. |
| [MatrixEquationNode](./matrixequationnode/) | Diese Klasse spezifiziert die Matrix‑Gleichung, die aus einem oder mehreren Elementen besteht, die in ein oder mehreren Zeilen und ein oder mehreren Spalten angeordnet sind. |
| [NaryEquationNode](./naryequationnode/) | Diese Klasse spezifiziert eine n‑stellige Operator‑Gleichung, die aus einem n‑stelligen Operator, einer Basis (oder Operanden) und optionalen oberen und unteren Grenzen besteht. |
| [RadicalEquationNode](./radicalequationnode/) | Diese Klasse spezifiziert die Radikal‑Gleichung, die aus einem optionalen Grad deg(EquationNodeType.Degree) und einer Basis besteht. |
| [SubSupEquationNode](./subsupequationnode/) | Diese Klasse spezifiziert eine Gleichung, die optional als Hoch- oder Tiefstellung dargestellt werden kann. Es gibt vier Hauptformen dieser Gleichung: Hochstellung, Tiefstellung, Hoch‑ und Tiefstellung links von der Basis sowie Hoch‑ und Tiefstellung rechts von der Basis. |
| [TextRunEquationNode](./textrunequationnode/) | Diese Klasse im Gleichungsknoten wird verwendet, um den tatsächlichen Inhalt (eine Sequenz mathematischen Textes) der Gleichung zu speichern. In der Regel ein Knotenobjekt pro Zeichen. |
| [UnknowEquationNode](./unknowequationnode/) | Gleichungsknotenklasse unbekannten Typs |
## Aufzählung

| Aufzählung | Beschreibung |
| --- | --- |
| [EquationCharacterPositionType](./equationcharacterpositiontype/) | Gibt die Position eines bestimmten Unterobjekts innerhalb seines Elternteils an |
| [EquationCombiningCharacterType](./equationcombiningcharactertype/) | Typ von Kombinationszeichen. |
| [EquationDelimiterShapeType](./equationdelimitershapetype/) | Dies gibt die Form der Trennzeichen im Trennzeichenobjekt an. |
| [EquationFractionType](./equationfractiontype/) | Dies gibt den Anzeigestil des Bruchstrichs an. |
| [EquationHorizontalJustificationType](./equationhorizontaljustificationtype/) | Dies gibt die standardmäßige horizontale Ausrichtung von Gleichungen im Dokument an. |
| [EquationLimitLocationType](./equationlimitlocationtype/) | Gibt den Grenzwertort auf einem Operator an. |
| [EquationMathematicalOperatorType](./equationmathematicaloperatortype/) | Typ mathematischer Operatoren |
| [EquationNodeType](./equationnodetype/) | Gleichungsknotentyp. Hinweis: (1)[1-99] Derzeit gibt es nur einen Knoten im Geltungsbereich, und sein Enumerationswert ist 1. Der von ihm spezifizierte Knoten wird verwendet, um mathematischen Text zu speichern. (2)[100-199] Gibt an, dass der Knoten ein Bestandteil einiger spezieller Funktionsknoten ist. (3)[200-] Gibt an, dass der Knoten einige Sonderfunktionen hat. |
| [EquationVerticalJustificationType](./equationverticaljustificationtype/) | Dies gibt die standardmäßige vertikale Ausrichtung von Gleichungen im Dokument an. |


