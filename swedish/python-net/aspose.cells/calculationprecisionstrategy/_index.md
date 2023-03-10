---
title: CalculationPrecisionStrategy uppräkning
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 1820
url: /sv/python-net/aspose.cells/calculationprecisionstrategy/
is_root: false
---
##  CalculationPrecisionStrategy uppräkning
Räknar upp strategier för att hantera beräkningsprecision.
På grund av precisionsproblemet med IEEE 754 Floating-Point Arithmetic, kanske vissa "till synes enkla" formler inte beräknas som det förväntade resultatet.
Såsom formeln "=-0,45+0,43+0,02", när man beräknar operander direkt med '+'-operatorn, är resultatet inte noll. För en sådan typ av precisionsproblem,
vissa speciella strategier kan ge det förväntade resultatet.



Typen CalculationPrecisionStrategy avslöjar följande medlemmar:

###  Fält
| Fält| Beskrivning|
| :- | :- |
| NONE | Ingen strategi tillämpas på beräkningen.<br/>När du beräknar använd bara det ursprungliga dubbelvärdet som operand och returnera resultatet direkt.<br/> Mest effektiv för prestanda och tillämplig i de flesta fall.|
| ROUND | Avrundar beräkningsresultatet med signifikanta siffror.|
| DECIMAL | Använder decimal som operander när det är möjligt.<br/> Mest ineffektivt för prestanda.|



###  Se även
* modul [aspose.cells](..)
