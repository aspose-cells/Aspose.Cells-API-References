---
title: "Worksheet.FilterString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet method. Ställer in filtret för kolumnen. Observera att vi ska anropa AddAutoFilter innan vi anropar filterString. Filterkriteriesträngen. Observera att vi använder komma som avgränsningstecken så cellvärdet du vill filtrera får inte innehålla komma. filterString10123456 betyder att kolumn 10 ska innehålla 123 eller 456. filterString10123 betyder att kolumn10 ska innehålla 123. Värdet separeras med komma t.ex. 123456789 eller abc"
type: docs
url: /sv/net/aspose.cells.griddesktop/worksheet/filterstring/
---
## Worksheet.FilterString method

Ställer in filtret för kolumnen. Observera att vi ska anropa AddAutoFilter innan filterString anropas. Filterkriteriesträngen. Observera att vi använder komma-&gt;"," som avgränsare, så cellvärdet du vill filtrera får inte innehålla komma. filterString(10,"123,456") betyder att kolumn 10 ska innehålla 123 eller 456, filterString(10,"123") betyder att kolumn 10 ska innehålla 123. Värdet separeras med komma, t.ex. 123,456,789 eller abc.

```csharp
public void FilterString(int column, string criteria)
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


