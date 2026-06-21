---
title: Aspose::Cells::Drawing::Equations Namespace
linktitle: Aspose::Cells::Drawing::Equations
second_title: Aspose.Cells für C++ API-Referenz
description: 'So verwenden Sie das Aspose::Cells::Drawing::Equations Namespace in C++.'
type: docs
weight: 600
url: /de/cpp/aspose.cells.drawing.equations/
---



## Klassen

| Klasse | Beschreibung |
| --- | --- |
| [AccentEquationNode](./accentequationnode/) | Diese Klasse definiert eine Akzentgleichung, die aus einer Basiskomponente und einem kombinierenden Diakritikum besteht. |
| [ArrayEquationNode](./arrayequationnode/) | Definiert die Equation-Array-Funktion, ein Objekt, das aus einer oder mehreren Gleichungen besteht. |
| [BarEquationNode](./barequationnode/) | Diese Klasse definiert die Balkengleichung, die aus einem Basisargument und einem Über- oder Unterstrich besteht. |
| [BorderBoxEquationNode](./borderboxequationnode/) | Diese Klasse definiert die [Border](../aspose.cells/border/) Box-Funktion, die aus einem um eine Gleichung gezeichneten Rahmen besteht. |
| [BoxEquationNode](./boxequationnode/) | Diese Klasse definiert die Box-Funktion, die verwendet wird, um Komponenten einer Gleichung zu gruppieren. |
| [DelimiterEquationNode](./delimiterequationnode/) | Diese Klasse definiert die Delimiter-Gleichung, die aus öffnenden und schließenden Delimitern (wie Klammern, geschweiften Klammern, eckigen Klammern und senkrechten Strichen) sowie einer darin enthaltenen Komponente besteht. Der Delimiter kann mehr als eine Komponente enthalten, wobei zwischen den Komponenten ein festgelegtes Trennzeichen steht. |
| [EquationComponentNode](./equationcomponentnode/) | Diese Klasse definiert die Komponenten einer Gleichung oder mathematischen Ausdrucks. Verschiedene Komponententypen werden zu unterschiedlichen Gleichungen kombiniert. Zum Beispiel besteht ein Bruch aus zwei Teilen, einer Zähler-Komponente und einer Nenner-Komponente. Für weitere Komponententypen siehe 'EquationNodeType'. |
| [EquationNode](./equationnode/) | Abstrakte Klasse zum Ableiten anderer Gleichungsknoten. |
| [EquationNodeParagraph](./equationnodeparagraph/) | Diese Klasse spezifiziert einen mathematischen Absatz, der ein oder mehrere MathEquationNode(OMath)-Elemente enthält. |
| [FractionEquationNode](./fractionequationnode/) | Diese Klasse spezifiziert die Bruchgleichung, die aus einem Zähler und einem Nenner besteht, die durch einen Bruchstrich getrennt sind. Der Bruchstrich kann je nach Bruch-Eigenschaften horizontal oder diagonal sein. Die Bruchgleichung wird außerdem verwendet, um die Stapelfunktion darzustellen, die ein Element über einem anderen platziert, ohne Bruchstrich. |
| [FunctionEquationNode](./functionequationnode/) | Diese Klasse spezifiziert die Function-Apply-Gleichung, die aus einem Funktionsnamen und einem darauf angewendeten Argument besteht. Die Typen der Namens‑ und Argumentkomponenten sind '[EquationNodeType.FunctionName](./equationnodetype/)' bzw. '[EquationNodeType.Base](./equationnodetype/)'. |
| [GroupCharacterEquationNode](./groupcharacterequationnode/) | Diese Klasse spezifiziert die Group-Character‑Funktion, die aus einem über oder unter dem Text platzierten Zeichen besteht, häufig mit dem Ziel, Elemente visuell zu gruppieren. |
| [LimLowUppEquationNode](./limlowuppequationnode/) | Diese Klasse spezifiziert die Grenzwertfunktion. |
| [MathematicalEquationNode](./mathematicalequationnode/) | Diese Klasse spezifiziert eine Gleichung oder einen mathematischen Ausdruck. Alle mathematischen Texte von Gleichungen oder mathematischen Ausdrücken werden von dieser Klasse enthalten. |
| [MatrixEquationNode](./matrixequationnode/) | Diese Klasse spezifiziert die Matrix‑Gleichung, die aus einem oder mehreren Elementen besteht, die in ein oder mehreren Zeilen und ein oder mehreren Spalten angeordnet sind. |
| [NaryEquationNode](./naryequationnode/) | Diese Klasse spezifiziert eine n‑stellige Operator‑Gleichung, die aus einem n‑stelligen Operator, einer Basis (oder einem Operanden) und optionalen oberen und unteren Grenzen besteht. |
| [RadicalEquationNode](./radicalequationnode/) | Diese Klasse spezifiziert die Radikal‑Gleichung, die aus einem optionalen Grad deg([EquationNodeType.Degree](./equationnodetype/)) und einer Basis besteht. |
| [SubSupEquationNode](./subsupequationnode/) | Diese Klasse spezifiziert eine Gleichung, die optional als Hoch- oder Tiefstellung dargestellt werden kann. Es gibt vier Hauptformen dieser Gleichung: Hochstellung, Tiefstellung, Hoch- und Tiefstellung links von der Basis sowie Hoch- und Tiefstellung rechts von der Basis. |
| [TextRunEquationNode](./textrunequationnode/) | Diese Klasse im Gleichungsknoten wird verwendet, um den tatsächlichen Inhalt (eine Sequenz mathematischer Texte) der Gleichung zu speichern. Üblicherweise ein Knotenobjekt pro Zeichen. |
| [UnknowEquationNode](./unknowequationnode/) | Gleichungsknotenklasse unbekannten Typs. |
## Enums

| Enum | Beschreibung |
| --- | --- |
| [EquationCharacterPositionType](./equationcharacterpositiontype/) | Gibt die Position eines bestimmten Unterobjekts innerhalb seines Elternteils an. |
| [EquationCombiningCharacterType](./equationcombiningcharactertype/) | Typ von Kombinationszeichen. |
| [EquationDelimiterShapeType](./equationdelimitershapetype/) | Dies gibt die Form der Trennzeichen im Trennzeichenobjekt an. |
| [EquationFractionType](./equationfractiontype/) | Dies gibt den Anzeigestil des Bruchstrichs an. |
| [EquationHorizontalJustificationType](./equationhorizontaljustificationtype/) | Dies gibt die standardmäßige horizontale Ausrichtung von Gleichungen im Dokument an. |
| [EquationLimitLocationType](./equationlimitlocationtype/) | Gibt den Grenzwertort auf einem Operator an. |
| [EquationMathematicalOperatorType](./equationmathematicaloperatortype/) | Typ mathematischer Operatoren. |
| [EquationNodeType](./equationnodetype/) | Gleichungsknoten‑Typ. Hinweis: (1)[1-99] Derzeit gibt es nur einen Knoten im Geltungsbereich, und sein Enumerationswert ist 1. Der von ihm spezifizierte Knoten wird verwendet, um mathematischen Text zu speichern. (2)[100-199] Zeigt an, dass der Knoten ein Bestandteil einiger spezieller Funktionsknoten ist. (3)[200-] Zeigt an, dass der Knoten einige Sonderfunktionen hat. |
| [EquationVerticalJustificationType](./equationverticaljustificationtype/) | Dies gibt die standardmäßige vertikale Ausrichtung von Gleichungen im Dokument an. |
