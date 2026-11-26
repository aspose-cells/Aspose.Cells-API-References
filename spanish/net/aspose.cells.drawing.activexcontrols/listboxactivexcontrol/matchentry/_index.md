---
title: "ListBoxActiveXControl.MatchEntry"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ListBoxActiveXControl propiedad. Indica cómo un ListBox o ComboBox busca en su lista mientras el usuario escribe"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/matchentry/
---
## ListBoxActiveXControl.MatchEntry property

Indica cómo un ListBox o ComboBox busca en su lista mientras el usuario escribe.

```csharp
public ControlMatchEntryType MatchEntry { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyMatchEntryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["A5"].PutValue("Date");

            // Agrega un control ListBox ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 5, 0, 1, 0, 100, 80);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Configura las propiedades del ListBox
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;
            listBox.MatchEntry = ControlMatchEntryType.FirstLetter;
            listBox.Value = "Apple;Banana;Cherry;Date";

            // Guarda el libro de trabajo
            workbook.Save("ListBoxMatchEntryDemo.xlsx");

            Console.WriteLine("ListBox with FirstLetter MatchEntry created successfully.");
        }
    }
}
```

### Ver también

* enum [ControlMatchEntryType](../../controlmatchentrytype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


