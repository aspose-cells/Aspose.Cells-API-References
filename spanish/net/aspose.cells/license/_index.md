---
title: "Clase License"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.License. Proporciona métodos para licenciar el componente"
type: docs
url: /es/net/aspose.cells/license/
---
## License class

Proporciona métodos para licenciar el componente.

```csharp
public class License
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [License](license/)() | Inicializa una nueva instancia de esta clase. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetLicense](../../aspose.cells/license/setlicense/#setlicense)(Stream) | Licencia el componente. |
| [SetLicense](../../aspose.cells/license/setlicense/#setlicense_1)(string) | Licencia el componente. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LicenseDemo
    {
        public static void LicenseExample()
        {
            // Crear una instancia de la clase License
            License license = new License();

            // Establecer la licencia usando el nombre de un archivo de licencia
            license.SetLicense("Aspose.Cells.NET.lic");

            // Alternativamente, establezca la licencia usando un flujo
            using (FileStream licenseStream = new FileStream("Aspose.Cells.NET.lic", FileMode.Open))
            {
                license.SetLicense(licenseStream);
            }

            // Código adicional para demostrar el uso de la funcionalidad licenciada de Aspose.Cells
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, Aspose.Cells!");

            // Guarde el libro de trabajo para verificar que la licencia se haya aplicado correctamente
            workbook.Save("LicensedWorkbook.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


