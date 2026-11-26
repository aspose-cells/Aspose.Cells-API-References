---
title: "WorkbookSettings.ProtectionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene el tipo de protección del libro de trabajo"
type: docs
url: /es/net/aspose.cells/workbooksettings/protectiontype/
---
## WorkbookSettings.ProtectionType property

Obtiene el tipo de protección del workbook.

```csharp
public ProtectionType ProtectionType { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyProtectionTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Proteger el libro de trabajo con el tipo de protección de Windows
            workbook.Protect(ProtectionType.Windows, "password123");
            
            // Demostrar la propiedad ProtectionType
            Console.WriteLine("Workbook protection type: " + workbook.Settings.ProtectionType);
            
            // Guarda el libro de trabajo
            workbook.Save("ProtectedWorkbook.xlsx");
            
            // Cargar el libro de trabajo guardado para verificar que el tipo de protección persista
            Workbook loadedWorkbook = new Workbook("ProtectedWorkbook.xlsx");
            Console.WriteLine("Loaded workbook protection type: " + loadedWorkbook.Settings.ProtectionType);
        }
    }
}
```

### Ver también

* enum [ProtectionType](../../protectiontype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


