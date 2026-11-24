---
title: "MainWeb.OnSubmitClientFunction"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MainWeb-Eigenschaft. Gibt die clientseitige Funktion an, die vor dem Absenden des Steuerelements aufgerufen wird, oder legt sie fest. Die clientseitige Funktion sollte wie folgt deklariert werden: function MyOnSubmitarg cancelEdit  return true Das Argument arg ist das Submit‑Argument und enthält den Befehl, der an den Server gesendet wird. cancelEdit ist ein boolescher Wert, der angibt, ob das Steuerelement die Benutzereingaben vor dem Absenden verworfen hat. Das Steuerelement fährt mit dem Absenden fort, wenn die Funktion true zurückgibt. Hinweis: Sie können den this‑Pointer in der clientseitigen Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst."
type: docs
url: /de/net/aspose.cells.gridweb/mainweb/onsubmitclientfunction/
---
## MainWeb.OnSubmitClientFunction property

Legt die Clientfunktion fest, die vor dem Absenden des Steuerelements auf der Clientseite aufgerufen wird, oder ruft sie ab. Die Clientfunktion sollte wie folgt deklariert werden: function MyOnSubmit(arg, cancelEdit) { return true;} Das Argument arg ist das Übermittlungsargument und enthält den Befehl, der an den Server gesendet wird. cancelEdit ist ein boolescher Wert, der angibt, ob das Steuerelement die Benutzereingabe vor dem Absenden verworfen hat. Das Steuerelement wird weiter senden, wenn die Funktion true zurückgibt. Hinweis: Sie können den "this"-Zeiger in der Clientfunktion verwenden, um auf das Grid-Steuerelement zu verweisen, das das Ereignis auslöst.

```csharp
public string OnSubmitClientFunction { get; set; }
```

### Siehe auch

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


