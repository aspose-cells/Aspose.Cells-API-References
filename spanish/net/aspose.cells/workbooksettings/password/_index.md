---
title: "WorkbookSettings.Password"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Representa la contraseña de cifrado del archivo del libro de trabajo"
type: docs
url: /es/net/aspose.cells/workbooksettings/password/
---
## WorkbookSettings.Password property

Representa la contraseña de cifrado del archivo Workbook.

```csharp
public string Password { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyPasswordDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            
            // Acceder a la primera hoja de cálculo y agregar algunos datos
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["C6"].PutValue("test encrypt.");
            
            // Establecer la contraseña para proteger el libro de trabajo
            wb.Settings.Password = "xixi";
            
            // Guarda el libro de trabajo
            wb.Save("output_with_password.ods");
            
            // Crear opciones de carga con contraseña para abrir el libro de trabajo protegido
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.Password = "xixi";
            
            // Abrir el libro de trabajo protegido con contraseña
            Workbook wbProtected = new Workbook("output_with_password.ods", loadOptions);
            
            // Verificar los datos
            Console.WriteLine("Cell value: " + wbProtected.Worksheets[0].Cells["C6"].Value);
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


