---
title: "ActiveXControlBase.Data"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ActiveXControlBase. Obtiene y establece los datos binarios del control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/data/
---
## ActiveXControlBase.Data property

Obtiene y establece los datos binarios del control.

```csharp
public virtual byte[] Data { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;
    using System.Drawing;

    public class ActiveXControlBasePropertyDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            cells["A2"].Value = "Sales";
            cells["A3"].Value = "Finance";
            cells["A4"].Value = "MIS";
            cells["A5"].Value = "R&D";
            cells["A6"].Value = "Marketing";
            cells["A7"].Value = "HRA";

            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 5, 0, 5, 0, 100, 200);
            shape.Name = "MyList";
            ListBoxActiveXControl list = (ListBoxActiveXControl)shape.ActiveXControl;

            list.ListFillRange = ("A3:A7");
            list.Value = ("Apple");
            list.LinkedCell = ("A1");
            list.ListStyle = (ControlListStyle.Option);
            list.SelectionType = (SelectionType.Multi);

            // Mostrar información inicial de la propiedad Data
            Console.WriteLine("Initial Data length: " + list.Data.Length);

            // Modificar las propiedades del control que afectan a Data
            list.BackOleColor = 0xFF0000;

            // Mostrar información actualizada de la propiedad Data
            Console.WriteLine("Modified Data length: " + list.Data.Length);

            // Guardar el libro de trabajo para demostrar los cambios persistentes
            workbook.Save("ActiveXControlDataDemo.xlsx");

        }
    }
}
```

### Ver también

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


