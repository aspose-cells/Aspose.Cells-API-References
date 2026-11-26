---
title: "AbstractLowCodeProtectionProvider.GetOpenPassword"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AbstractLowCodeProtectionProvider. Obtiene la contraseña para abrir el archivo de hoja de cálculo"
type: docs
url: /es/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getopenpassword/
---
## AbstractLowCodeProtectionProvider.GetOpenPassword method

Obtiene la contraseña para abrir el archivo de hoja de cálculo.

```csharp
public virtual string GetOpenPassword()
```

### Valor de retorno

Contraseña para abrir el archivo de hoja de cálculo. Vacío significa que no hay protección al abrir el archivo.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetOpenPasswordDemo
    {
        public static void Run()
        {
            try
            {
                // Crear una instancia del proveedor de protección
                var protectionProvider = new DemoProtectionProvider();

                // Llamar al método GetOpenPassword para obtener la contraseña
                string password = protectionProvider.GetOpenPassword();

                // Crear un nuevo libro de trabajo y aplicar la contraseña
                Workbook workbook = new Workbook("sample.xlsx");
                workbook.Settings.Password = password;

                // Guardar el libro de trabajo protegido con contraseña
                workbook.Save("MethodGetOpenPasswordDemo.xlsx");

                Console.WriteLine($"Workbook protected with open password: {password}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing demo: {ex.Message}");
            }
        }
    }

    public class DemoProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetOpenPassword()
        {
            return "AsposeDemo123!";
        }
    }
}
```

### Ver también

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


