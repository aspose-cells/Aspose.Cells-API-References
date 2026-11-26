---
title: "Name.IsVisible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Name. Indica si el nombre es visible"
type: docs
url: /es/net/aspose.cells/name/isvisible/
---
## Name.IsVisible property

Indica si el nombre es visible.

```csharp
public bool IsVisible { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un rango con nombre visible
            int visibleIndex = workbook.Worksheets.Names.Add("VisibleRange");
            Name visibleName = workbook.Worksheets.Names[visibleIndex];
            visibleName.RefersTo = "=Sheet1!$A$1:$B$2";
            visibleName.IsVisible = true;
            
            // Crear un rango con nombre oculto
            int hiddenIndex = workbook.Worksheets.Names.Add("HiddenRange");
            Name hiddenName = workbook.Worksheets.Names[hiddenIndex];
            hiddenName.RefersTo = "=Sheet1!$C$1:$D$2";
            hiddenName.IsVisible = false;
            
            // Demostrar la propiedad IsVisible
            Console.WriteLine("VisibleRange IsVisible: " + visibleName.IsVisible);
            Console.WriteLine("HiddenRange IsVisible: " + hiddenName.IsVisible);
            
            // Guarda el libro de trabajo
            workbook.Save("NameVisibilityDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


