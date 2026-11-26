---
title: "Style.IsFormulaHidden"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Representa si la fórmula se ocultará cuando la hoja de cálculo esté protegida"
type: docs
url: /es/net/aspose.cells/style/isformulahidden/
---
## Style.IsFormulaHidden property

Representa si la fórmula se ocultará cuando la hoja de cálculo esté protegida.

```csharp
public bool IsFormulaHidden { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsFormulaHiddenDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear un estilo con IsFormulaHidden establecido en verdadero
            Style style = workbook.CreateStyle();
            style.IsFormulaHidden = true;
            
            // Aplicar el estilo a una celda
            cells["A1"].SetStyle(style);
            cells["A1"].Formula = "=1+1";

            // Crear otro estilo con IsFormulaHidden establecido en falso
            Style style2 = workbook.CreateStyle();
            style2.IsFormulaHidden = false;
            
            // Aplicar el segundo estilo a otra celda
            cells["B1"].SetStyle(style2);
            cells["B1"].Formula = "=2+2";

            // Proteger la hoja de cálculo para ver el efecto
            worksheet.Protect(ProtectionType.All, "password", null);

            // Guarda el libro de trabajo
            workbook.Save("IsFormulaHiddenDemo.xlsx");

            Console.WriteLine("Workbook saved with IsFormulaHidden examples.");
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


