---
title: "AbstractLowCodeProtectionProvider.GetWritePassword"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AbstractLowCodeProtectionProvider. Obtiene la contraseña para modificar el archivo de hoja de cálculo"
type: docs
url: /es/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getwritepassword/
---
## AbstractLowCodeProtectionProvider.GetWritePassword method

Obtiene la contraseña para modificar el archivo de hoja de cálculo.

```csharp
public virtual string GetWritePassword()
```

### Valor de retorno

Contraseña para modificar el archivo de hoja de cálculo. Vacío significa que no hay protección para modificar el archivo.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWritePasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Crea una instancia del proveedor de protección personalizado
            var protectionProvider = new CustomProtectionProvider();

            try
            {
                // Llamar explícitamente a GetWritePassword y mostrar el resultado
                string writePassword = protectionProvider.GetWritePassword();
                Console.WriteLine($"Retrieved write password: {writePassword}");

                // Guardar libro de trabajo - aplicar protección de escritura directamente
                workbook.Settings.WriteProtection.Password = writePassword;
                workbook.Save("MethodGetWritePasswordDemo.xlsx");
                Console.WriteLine("Workbook saved with write protection password.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetWritePassword method: {ex.Message}");
            }
        }

    }

    // Implementación personalizada del proveedor de protección
    public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetWritePassword()
        {
            return "AsposeTestPassword123!";
        }

        // Implementar otros métodos requeridos con devoluciones predeterminadas
        public override string GetOpenPassword() => null;
        public override string GetWorkbookPassword() => null;
        public override ProtectionType GetWorkbookProtectionType() => ProtectionType.None;
        public override string GetWorksheetPassword(string sheetName) => null;
        public override ProtectionType GetWorksheetProtectionType(string sheetName) => ProtectionType.None;
    }
}
```

### Ver también

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


