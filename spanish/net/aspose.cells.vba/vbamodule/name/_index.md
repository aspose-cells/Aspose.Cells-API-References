---
title: "VbaModule.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VbaModule. Obtiene y establece el nombre del módulo"
type: docs
url: /es/net/aspose.cells.vba/vbamodule/name/
---
## VbaModule.Name property

Obtiene y establece el nombre del módulo.

```csharp
public string Name { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();

            // Agregar una hoja de cálculo y obtener su módulo VBA
            Worksheet sheet = wb.Worksheets[0];
            int moduleIndex = wb.VbaProject.Modules.Add(sheet);
            VbaModule module = wb.VbaProject.Modules[moduleIndex];

            // Establecer el nombre del módulo
            module.Name = "Sheet1";

            // Agregar código VBA simple al módulo
            string vbaCode = "Private Sub Worksheet_SelectionChange(ByVal Target As Range)\r\n" +
                             "    MsgBox \"Sheet name: \" & Me.Name\r\n" +
                             "End Sub\r\n";
            module.Codes = vbaCode;

            // Guardar en un flujo de memoria (para demostración)
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsm);
            }
        }
    }
}
```

### Ver también

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


