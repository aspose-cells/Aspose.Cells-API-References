---
title: "GridValidation.GetListValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridValidation metod. Hämta värdet för listan av valideringen för den specificerade cellen"
type: docs
url: /sv/net/aspose.cells.gridweb.data/gridvalidation/getlistvalue/
---
## GridValidation.GetListValue method

Hämta värdet för listan av valideringen för den angivna cellen.

```csharp
public object GetListValue(int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindexet. |
| column | Int32 | Kolumnindexet. |

### Returvärde

Värdet för att skapa listan för denna validering för den specificerade cellen. Om listan refererar till ett område, kommer det returnerade värdet att vara ett ReferredArea-objekt; annars kan det returnerade värdet vara null, object[] eller ett enkelt objekt.

### Anmärkningar

Endast för validering vars typ är List och som har tillämpats på den angivna cellen, annars returneras null.

### Se även

* class [GridValidation](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


