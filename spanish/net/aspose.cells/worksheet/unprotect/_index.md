---
title: "Worksheet.Unprotect"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Worksheet method. Desprotege la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/unprotect/
---
## Unprotect() {#unprotect}

Desprotege la hoja de cálculo.

```csharp
public void Unprotect()
```

### Observaciones

Este método desprotege la hoja de cálculo que está protegida sin contraseña.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodUnprotectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Proteger la hoja de cálculo con una contraseña
            worksheet.Protect(ProtectionType.All, "password123", null);
            Console.WriteLine("Worksheet is protected: " + worksheet.IsProtected);
            
            try
            {
                // Desproteger la hoja de cálculo sin contraseña (debe fallar)
                worksheet.Unprotect();
                Console.WriteLine("Worksheet unprotected without password: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect without password: " + ex.Message);
            }

            try
            {
                // Desproteger la hoja de cálculo con contraseña incorrecta (debe fallar)
                worksheet.Unprotect("wrongpassword");
                Console.WriteLine("Worksheet unprotected with wrong password: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect with wrong password: " + ex.Message);
            }

            try
            {
                // Desproteger la hoja de cálculo con la contraseña correcta
                worksheet.Unprotect("password123");
                Console.WriteLine("Worksheet successfully unprotected: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect: " + ex.Message);
            }
            
            // Guardar el resultado
            workbook.Save("WorksheetMethodUnprotectDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Unprotect(string) {#unprotect_1}

Desprotege la hoja de cálculo.

```csharp
public void Unprotect(string password)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| contraseña | String | Contraseña |

### Observaciones

Si la hoja de cálculo está protegida sin una contraseña, puede establecer un valor nulo o una cadena vacía en el parámetro contraseña.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodUnprotectWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Proteger la hoja de cálculo con contraseña y tipo de protección predeterminado
            worksheet.Protect(ProtectionType.All, "test", null);
            
            // Desproteger la hoja de cálculo con contraseña
            worksheet.Unprotect("test");
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


