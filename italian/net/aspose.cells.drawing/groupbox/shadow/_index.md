---
title: "GroupBox.Shadow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GroupBox. Indica se il groupbox ha l'ombra"
type: docs
url: /it/net/aspose.cells.drawing/groupbox/shadow/
---
## GroupBox.Shadow property

Indica se il groupbox ha l'ombra.

```csharp
public bool Shadow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class GroupBoxPropertyShadowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un group box con ombra
            GroupBox groupBoxWithShadow = worksheet.Shapes.AddGroupBox(1, 0, 1, 0, 200, 150);
            groupBoxWithShadow.Shadow = true;
            groupBoxWithShadow.Text = "GroupBox with Shadow";
            
            // Aggiungi un group box senza ombra
            GroupBox groupBoxWithoutShadow = worksheet.Shapes.AddGroupBox(1, 2, 1, 0, 200, 150);
            groupBoxWithoutShadow.Shadow = false;
            groupBoxWithoutShadow.Text = "GroupBox without Shadow";
            
            // Aggiungi pulsanti radio all'interno dei group box per dimostrare il raggruppamento
            RadioButton radio1 = worksheet.Shapes.AddRadioButton(3, 0, 2, 0, 30, 100);
            radio1.Text = "Option 1";
            radio1.LinkedCell = "A1";
            
            RadioButton radio2 = worksheet.Shapes.AddRadioButton(6, 0, 2, 0, 30, 100);
            radio2.Text = "Option 2";
            radio2.LinkedCell = "A1";
            
            // Raggruppa le forme
            Shape[] shapes = { groupBoxWithShadow, radio1, radio2 };
            worksheet.Shapes.Group(shapes);
            
            // Salva la cartella di lavoro
            workbook.Save("GroupBoxShadowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [GroupBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


