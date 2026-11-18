---
title: "FormulaParseOptions klass"
linktitle: "FormulaParseOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "FormulaParseOptions klass. Inkapslar objektet som representerar formulaparseoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/formulaparseoptions/
---

## FormulaParseOptions class

Representerar alternativ vid tolkning av formel.

```go

type FormulaParseOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewFormulaParseOptions](./newformulaparseoptions/) | Standardkonstruktor. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetLocaleDependent](./getlocaledependent/) | Om formeln är lokalanpassad. Standard är falskt. |
| [SetLocaleDependent](./setlocaledependent/) | Om formeln är lokalanpassad. Standard är falskt. |
| [GetR1C1Style](./getr1c1style/) | Om formeln är i R1C1-referensstil. Standard är falskt. |
| [SetR1C1Style](./setr1c1style/) | Om formeln är i R1C1-referensstil. Standard är falskt. |
| [GetCheckAddIn](./getcheckaddin/) | Om tillägg ska kontrolleras i befintliga externa länkar i den aktuella arbetsboken för användardefinierade funktioner utan extern länk. Standard är sant (om en användardefinierad funktion matchar ett tillägg i befintliga externa länkar, tas det som tillägget). |
| [SetCheckAddIn](./setcheckaddin/) | Om tillägg ska kontrolleras i befintliga externa länkar i den aktuella arbetsboken för användardefinierade funktioner utan extern länk. Standard är sant (om en användardefinierad funktion matchar ett tillägg i befintliga externa länkar, tas det som tillägget). |
| [GetParse](./getparse/) | Om given formel ska parsas. Standard är sant. Om den är falsk, behålls den givna formelsträngen oförändrad för cellen tills användaren anropar andra metoder för att parsas eller parsad formeldatat krävs av andra operationer såsom beräkning av formler. |
| [SetParse](./setparse/) | Om given formel ska parsas. Standard är sant. Om den är falsk, behålls den givna formelsträngen oförändrad för cellen tills användaren anropar andra metoder för att parsas eller parsad formeldatat krävs av andra operationer såsom beräkning av formler. |
| [GetCustomFunctionDefinition](./getcustomfunctiondefinition/) | Definition för parsning av anpassade funktioner. |
| [SetCustomFunctionDefinition](./setcustomfunctiondefinition/) | Definition för parsning av anpassade funktioner. |
