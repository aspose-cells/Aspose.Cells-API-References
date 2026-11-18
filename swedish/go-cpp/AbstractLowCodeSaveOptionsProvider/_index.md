---
title: "AbstractLowCodeSaveOptionsProvider-klass"
linktitle: "AbstractLowCodeSaveOptionsProvider"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "AbstractLowCodeSaveOptionsProvider-klass. Inkapslar objektet som representerar abstractlowcodesaveoptionsprovider i Go."
type: docs
weight: 200
url: /sv/go-cpp/abstractlowcodesaveoptionsprovider/
---

## AbstractLowCodeSaveOptionsProvider class

Implementering för att tillhandahålla flera sparaalternativ för processer som kräver flera utdata. Till exempel <see cref="SpreadsheetSplitter"/>-funktionen kräver flera destinationer för att spara de delade filerna.

```go

type AbstractLowCodeSaveOptionsProvider struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetSaveOptions](./getsaveoptions/) | Hämtar sparalternativen från vilka utdatainställningarna för den aktuella delade delen erhålls. Att returnera null betyder att hoppa över den givna delen. |
| [Finish](./finish/) | Frigör resurser efter bearbetning av den aktuella delade delen. |
