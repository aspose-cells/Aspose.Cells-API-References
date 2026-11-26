---
title: "WorkbookSettings.WarningCallback"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene o establece la devolución de llamada de advertencia"
type: docs
url: /es/net/aspose.cells/workbooksettings/warningcallback/
---
## WorkbookSettings.WarningCallback property

Obtiene o establece la devolución de llamada de advertencia.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Establecer la devolución de llamada de advertencia
            workbook.Settings.WarningCallback = new WarningCallbackImplementation();

            // Crear una hoja de cálculo con un escenario potencial de advertencia (rango con nombre duplicado)
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test");
            
            // Esto activará una advertencia sobre un nombre duplicado
            int index1 = workbook.Worksheets.Names.Add("TestRange");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$A$1";
            
            int index2 = workbook.Worksheets.Names.Add("TestRange");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$A$1";

            // Guardar el libro de trabajo (activará la devolución de llamada de advertencia)
            workbook.Save("WarningCallbackExample.xlsx");
        }
    }

    public class WarningCallbackImplementation : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine($"Warning: {warningInfo.WarningType}, Description: {warningInfo.Description}");
        }
    }
}
```

### Ver también

* interface [IWarningCallback](../../iwarningcallback/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


