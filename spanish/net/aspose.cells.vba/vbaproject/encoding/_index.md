---
title: "VbaProject.Encoding"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VbaProject. Obtiene y establece la codificación del proyecto VBA"
type: docs
url: /es/net/aspose.cells.vba/vbaproject/encoding/
---
## VbaProject.Encoding property

Obtiene y establece la codificación del proyecto VBA.

```csharp
public Encoding Encoding { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Vba;
using System.Security.Cryptography.X509Certificates;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyEncodingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Inicializar proyecto VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Establecer propiedades del proyecto VBA incluyendo la codificación
            vbaProject.Name = "TestVbaProject";
            vbaProject.Encoding = Encoding.UTF8;

            // Agregar un módulo al proyecto VBA
            vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");

            // Guardar el libro con el proyecto VBA
            workbook.Save("VbaProjectEncodingDemo.xlsm");
        }
    }
}
```

### Ver también

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


