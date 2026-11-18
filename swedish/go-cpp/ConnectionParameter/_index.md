---
title: "ConnectionParameter-klass"
linktitle: "ConnectionParameter"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "ConnectionParameter-klass. Inkapslar objektet som representerar connectionparameter i Go."
type: docs
weight: 200
url: /sv/go-cpp/connectionparameter/
---

## ConnectionParameter class

Specificerar egenskaper för alla parametrar som används med externa datakopplingar. Parametrar är giltiga för ODBC‑ och webbfrågor.

```go

type ConnectionParameter struct  {
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
| [GetSqlType](./getsqltype/) | SQL-datatyp för parametern. Endast giltig för ODBC-källor. |
| [SetSqlType](./setsqltype/) | SQL-datatyp för parametern. Endast giltig för ODBC-källor. |
| [GetRefreshOnChange](./getrefreshonchange/) | Flagga som anger om frågan ska uppdateras automatiskt när innehållet i en cell som tillhandahåller parametervärdet ändras. Om true, uppdateras extern data med det nya parametervärdet varje gång en förändring sker. Om false, uppdateras extern data endast när användaren begär det, eller när någon annan händelse triggar en uppdatering (t.ex. arbetsbok öppnad). |
| [SetRefreshOnChange](./setrefreshonchange/) | Flagga som anger om frågan ska uppdateras automatiskt när innehållet i en cell som tillhandahåller parametervärdet ändras. Om true, uppdateras extern data med det nya parametervärdet varje gång en förändring sker. Om false, uppdateras extern data endast när användaren begär det, eller när någon annan händelse triggar en uppdatering (t.ex. arbetsbok öppnad). |
| [GetPrompt](./getprompt/) | Promptsträng för parametern. Presenteras för kalkylbladsanvändaren tillsammans med inmatnings‑UI för att samla in parametervärdet innan den externa datan uppdateras. Används endast när parameterType = prompt. |
| [SetPrompt](./setprompt/) | Promptsträng för parametern. Presenteras för kalkylbladsanvändaren tillsammans med inmatnings‑UI för att samla in parametervärdet innan den externa datan uppdateras. Används endast när parameterType = prompt. |
| [GetType](./gettype/) | Typ av parameter som används. Om parameterType=value, används värdet från boolean, double, integer eller string. I detta fall förväntas endast ett av {boolean, double, integer, or string} specificeras. |
| [SetType](./settype/) | Typ av parameter som används. Om parameterType=value, används värdet från boolean, double, integer eller string. I detta fall förväntas endast ett av {boolean, double, integer, or string} specificeras. |
| [GetName](./getname/) | Namnet på parametern. |
| [SetName](./setname/) | Namnet på parametern. |
| [GetCellReference](./getcellreference/) | Cellreferens som anger vilket cellvärde som ska användas för frågeparametern. Används endast när parameterType är cell. |
| [SetCellReference](./setcellreference/) | Cellreferens som anger vilket cellvärde som ska användas för frågeparametern. Används endast när parameterType är cell. |
| [GetValue](./getvalue/) | Icke‑heltaligt numeriskt värde, heltalsvärde, strängvärde eller booleskt värde att använda som frågeparameter. Används endast när parameterType är value. |
| [SetValue](./setvalue/) | Icke‑heltaligt numeriskt värde, heltalsvärde, strängvärde eller booleskt värde att använda som frågeparameter. Används endast när parameterType är value. |
