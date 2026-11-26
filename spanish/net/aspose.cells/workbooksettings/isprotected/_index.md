---
title: "WorkbookSettings.IsProtected"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "propiedad WorkbookSettings. Obtiene un valor que indica si la estructura o la ventana del Workbook está protegida"
type: docs
url: /es/net/aspose.cells/workbooksettings/isprotected/
---
## WorkbookSettings.IsProtected property

Obtiene un valor que indica si la estructura o la ventana del libro están protegidas.

```csharp
public bool IsProtected { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsProtectedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la configuración del libro de trabajo
            WorkbookSettings settings = workbook.Settings;
            
            // Verifica si el libro está protegido
            Console.WriteLine("Workbook is protected: " + settings.IsProtected);
            
            // Proteger el libro de trabajo con una contraseña
            settings.Password = "password123";
            
            // Verificar el estado de protección
            Console.WriteLine("Workbook is protected: " + settings.IsProtected);
            
            // Guardar el libro de trabajo protegido
            workbook.Save("ProtectedWorkbook.xlsx", SaveFormat.Xlsx);
            
            // Abre el libro protegido
            Workbook protectedWorkbook = new Workbook("ProtectedWorkbook.xlsx");
            
            // Verifica el estado de protección del libro cargado
            Console.WriteLine("Loaded workbook is protected: " + protectedWorkbook.Settings.IsProtected);
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


