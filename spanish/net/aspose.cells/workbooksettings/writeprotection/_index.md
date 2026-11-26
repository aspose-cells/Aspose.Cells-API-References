---
title: "WorkbookSettings.WriteProtection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Proporciona acceso a las opciones de protección contra escritura del libro"
type: docs
url: /es/net/aspose.cells/workbooksettings/writeprotection/
---
## WorkbookSettings.WriteProtection property

Proporciona acceso a las opciones de protección contra escritura del libro de trabajo.

```csharp
public WriteProtection WriteProtection { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWriteProtectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Establecer propiedades de protección contra escritura
            workbook.Settings.WriteProtection.Password = "test123";
            workbook.Settings.WriteProtection.Author = "John Doe";
            workbook.Settings.WriteProtection.RecommendReadOnly = true;

            // Guarda el libro de trabajo
            string outputPath = "WriteProtectionDemo.xlsx";
            workbook.Save(outputPath);

            // Cargue el libro de trabajo guardado para verificar las propiedades
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Mostrar las propiedades de protección contra escritura
            Console.WriteLine("Author: " + loadedWorkbook.Settings.WriteProtection.Author);
            Console.WriteLine("ReadOnly Recommended: " + loadedWorkbook.Settings.WriteProtection.RecommendReadOnly);
        }
    }
}
```

### Ver también

* class [WriteProtection](../../writeprotection/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


