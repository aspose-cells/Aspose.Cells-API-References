---
title: "Style.Style"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Konstruktor. Initialisiert eine neue Instanz der Style-Klasse."
type: docs
url: /de/net/aspose.cells/style/style/
---
## Style constructor

Initialisiert eine neue Instanz der [`Style`](../)-Klasse.

```csharp
[Obsolete("Use CellsFactory.CreateStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Style()
```

### Hinweise

HINWEIS: Dieser Konstruktor ist jetzt veraltet. Verwenden Sie stattdessen die Methode CellsFactory.CreateStyle(). Diese Eigenschaft wird 6 Monate nach Oktober 2016 entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodCtorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie einen Style mithilfe des Konstruktors.
            Style style = new Style();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.Solid;

            // Wende den Stil auf eine Zelle an
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Styled Text");
            cell.SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("StyleConstructorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


