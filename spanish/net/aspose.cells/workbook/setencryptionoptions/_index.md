---
title: "Workbook.SetEncryptionOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Workbook. Establecer opciones de cifrado"
type: docs
url: /es/net/aspose.cells/workbook/setencryptionoptions/
---
## Workbook.SetEncryptionOptions method

Establecer opciones de cifrado.

```csharp
public void SetEncryptionOptions(EncryptionType encryptionType, int keyLength)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| encryptionType | EncryptionType | El tipo de cifrado. |
| keyLength | Int32 | La longitud de la clave. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetEncryptionOptionsWithEncryptionTypeInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunos datos a la hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Encryption");
            
            // Establecer contraseña y opciones de cifrado
            workbook.Settings.Password = "1234";
            workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, 128);
            
            // Guardar el libro de trabajo cifrado
            workbook.Save("EncryptedWorkbook.xls", SaveFormat.Excel97To2003);
            
            // Verificar cargando el libro de trabajo cifrado
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.Password = "1234";
            Workbook encryptedWorkbook = new Workbook("EncryptedWorkbook.xls", loadOptions);
            
            Console.WriteLine("Workbook encrypted and loaded successfully.");
        }
    }
}
```

### Ver también

* enum [EncryptionType](../../encryptiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


