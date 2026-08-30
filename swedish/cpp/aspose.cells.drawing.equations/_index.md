---
title: Aspose::Cells::Drawing::Equations namespace
linktitle: Aspose::Cells::Drawing::Equations
second_title: Aspose.Cells för C++ API-referens
description: 'Hur man använder Aspose::Cells::Drawing::Equations-namespace i C++.'
type: docs
weight: 600
url: /sv/cpp/aspose.cells.drawing.equations/
---



## Klasser

| Klass | Beskrivning |
| --- | --- |
| [AccentEquationNode](./accentequationnode/) | Denna klass specificerar en accentekvation, bestående av en baskomponent och ett kombinerande diakritiskt tecken. |
| [ArrayEquationNode](./arrayequationnode/) | Specificerar Equation-Array-funktionen, ett objekt bestående av en eller flera ekvationer. |
| [BarEquationNode](./barequationnode/) | Denna klass specificerar bar equation, bestående av ett basargument och ett överstreck eller understreck. |
| [BorderBoxEquationNode](./borderboxequationnode/) | Denna klass specificerar [Border](../aspose.cells/border/) Box-funktionen, bestående av en ram ritad runt en ekvation. |
| [BoxEquationNode](./boxequationnode/) | Denna klass specificerar box-funktionen, som används för att gruppera komponenter i en ekvation. |
| [DelimiterEquationNode](./delimiterequationnode/) | Denna klass specificerar delimiterekvationen, bestående av öppnings- och stängningsavgränsare (såsom parenteser, klammerparenteser, hakparenteser och vertikala streck), samt en komponent som finns inuti. Avgränsaren kan ha mer än en komponent, med ett angivet separator‑tecken mellan varje komponent. |
| [EquationComponentNode](./equationcomponentnode/) | Denna klass specificerar komponenterna i en ekvation eller matematisk uttryck. Olika typer av komponenter kombineras i olika ekvationer. Till exempel består en bråkdel av två delar, en täljarkomponent och en nämnarkomponent. För fler komponenttyper, se 'EquationNodeType'. |
| [EquationNode](./equationnode/) | Abstrakt klass för att härleda andra ekvationsnoder. |
| [EquationNodeParagraph](./equationnodeparagraph/) | Denna klass specificerar ett matematiskt stycke som innehåller ett eller flera MathEquationNode(OMath)-element. |
| [FractionEquationNode](./fractionequationnode/) | Denna klass specificerar bråklikheten, bestående av en täljare och en nämnare separerade av ett bråkstreck. Bråkstrecket kan vara horisontellt eller diagonalt, beroende på bråkegenskaperna. Bråklikheten används också för att representera stapelfunktionen, som placerar ett element ovanför ett annat, utan bråkstreck. |
| [FunctionEquationNode](./functionequationnode/) | Denna klass specificerar Function-Apply‑ekvationen, som består av ett funktionsnamn och ett argument som påverkas. Typerna för namn‑ och argumentkomponenterna är '[EquationNodeType.FunctionName](./equationnodetype/)' respektive '[EquationNodeType.Base](./equationnodetype/)' |
| [GroupCharacterEquationNode](./groupcharacterequationnode/) | Denna klass specificerar Group-Character‑funktionen, bestående av ett tecken som ritas ovanför eller under text, ofta för att visuellt gruppera objekt. |
| [LimLowUppEquationNode](./limlowuppequationnode/) | Denna klass specificerar gränsfunktionen. |
| [MathematicalEquationNode](./mathematicalequationnode/) | Denna klass specificerar en ekvation eller ett matematiskt uttryck. All matematisk text för ekvationer eller matematiska uttryck innehålls av denna klass. |
| [MatrixEquationNode](./matrixequationnode/) | Denna klass specificerar Matrix‑ekvationen, bestående av ett eller flera element ordnade i en eller flera rader och en eller flera kolumner. |
| [NaryEquationNode](./naryequationnode/) | Denna klass specificerar en n‑är operator‑ekvation som består av en n‑är operator, en bas (eller operand) samt valfria övre och nedre gränser. |
| [RadicalEquationNode](./radicalequationnode/) | Denna klass specificerar radikal‑ekvationen, bestående av en valfri grad deg([EquationNodeType.Degree](./equationnodetype/)) och en bas. |
| [SubSupEquationNode](./subsupequationnode/) | Denna klass specificerar en ekvation som valfritt kan vara upphöjd eller nedsänkt. Det finns fyra huvudformer av denna ekvation: upphöjd, nedsänkt, upphöjd och nedsänkt placerade till vänster om basen, samt upphöjd och nedsänkt placerade till höger om basen. |
| [TextRunEquationNode](./textrunequationnode/) | Denna klass i ekvationsnoden används för att lagra det faktiska innehållet (en sekvens av matematisk text) i ekvationen. Vanligtvis ett nodobjekt per tecken. |
| [UnknowEquationNode](./unknowequationnode/) | Ekvationsnodsklass av okänd typ. |
## Enums

| Enum | Beskrivning |
| --- | --- |
| [EquationCharacterPositionType](./equationcharacterpositiontype/) | Specificerar positionen för ett särskilt delobjekt inom dess förälder. |
| [EquationCombiningCharacterType](./equationcombiningcharactertype/) | Typ av kombinerande tecken. |
| [EquationDelimiterShapeType](./equationdelimitershapetype/) | Detta specificerar formen på avgränsare i avgränsarobjektet. |
| [EquationFractionType](./equationfractiontype/) | Detta specificerar visningsstilen för bråkstrecket. |
| [EquationHorizontalJustificationType](./equationhorizontaljustificationtype/) | Detta specificerar standardhorisontell justering av ekvationer i dokumentet. |
| [EquationLimitLocationType](./equationlimitlocationtype/) | Specificerar gränsplatsen på en operator. |
| [EquationMathematicalOperatorType](./equationmathematicaloperatortype/) | Typ av matematiska operatorer. |
| [EquationNodeType](./equationnodetype/) | Ekvationsnodtyp. Observera: (1)[1-99] För närvarande finns det bara en nod i området, och dess uppräkningsvärde är 1. Noden den specificerar används för att lagra matematisk text. (2)[100-199] Anger att noden är en komponent i vissa specialfunktioner. (3)[200-] Anger att noden har vissa specialfunktioner. |
| [EquationVerticalJustificationType](./equationverticaljustificationtype/) | Detta specificerar standardvertikal justering av ekvationer i dokumentet. |
