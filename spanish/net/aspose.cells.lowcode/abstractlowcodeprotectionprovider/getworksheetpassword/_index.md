---
title: "AbstractLowCodeProtectionProvider.GetWorksheetPassword"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AbstractLowCodeProtectionProvider. Obtiene la contraseña para proteger la hoja de cálculo especificada"
type: docs
url: /es/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetpassword/
---
## AbstractLowCodeProtectionProvider.GetWorksheetPassword method

Obtiene la contraseña para proteger la hoja de cálculo especificada.

```csharp
public virtual string GetWorksheetPassword(string sheetName)
```

### Valor de retorno

Contraseña para proteger la hoja de cálculo especificada.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWorksheetPasswordWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            string sheetName = worksheet.Name;

            // Crea una instancia del proveedor de protección personalizado
            var provider = new CustomProtectionProvider();

            try
            {
                // Llamar a GetWorksheetPassword con el nombre de la hoja de cálculo
                string password = provider.GetWorksheetPassword(sheetName);

                // Aplicar protección a la hoja de cálculo usando la contraseña obtenida
                worksheet.Protect(ProtectionType.All, password, null);

                Console.WriteLine($"Protected worksheet '{sheetName}' with password: {password}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetWorksheetPassword: {ex.Message}");
            }

            // Guardar el libro de trabajo protegido
            workbook.Save("WorksheetPasswordDemo.xlsx");

        }
    }

    // Implementación personalizada que devuelve la contraseña basada en el nombre de la hoja
    public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public new string GetWorksheetPassword(string sheetName)
        {
            // Lógica simple de generación de contraseñas para demostración
            return $"pw_{sheetName}";
        }
    }
}
```

### Ver también

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


