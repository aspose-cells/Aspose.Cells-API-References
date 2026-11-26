---
title: "SpreadsheetLocker.Process"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SpreadsheetLocker. Bloquea el archivo de hoja de cálculo con la configuración especificada"
type: docs
url: /es/net/aspose.cells.lowcode/spreadsheetlocker/process/
---
## Process(string, string, string, string) {#process_3}

Bloquea el archivo de hoja de cálculo con la configuración especificada.

```csharp
public static void Process(string templateFile, string resultFile, string openPassword, 
    string writePassword)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| templateFile | String | El archivo de plantilla a bloquear |
| resultFile | String | El archivo resultante |
| openPassword | String | Contraseña para el cifrado del archivo |
| writePassword | String | Contraseña para la protección de la modificación de la hoja de cálculo |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class SpreadsheetLockerMethodProcessWithStringStringStringStringDemo
    {
        public static void Run()
        {           
            string templatePath = "template.xlsx";            
            // Preparar la ruta del archivo de resultado
            string resultPath = "secured_spreadsheet.xlsx";

            try
            {
                // Ejecutar el método Process con parámetros de cadena directamente usando el tipo
                SpreadsheetLocker.Process(
                    templateFile: templatePath,
                    resultFile: resultPath,
                    openPassword: "Open@123",
                    writePassword: "Write@456"
                );

                Console.WriteLine($"Spreadsheet secured successfully. Saved to: {Path.GetFullPath(resultPath)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error securing spreadsheet: {ex.Message}");
            }
            finally
            {
                // Limpiar la plantilla temporal
                if (File.Exists(templatePath))
                {
                    File.Delete(templatePath);
                }
            }
        }
    }
}
```

### Ver también

* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, string, string) {#process_1}

Bloquea el archivo de hoja de cálculo con la configuración especificada.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    string openPassword, string writePassword)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Opciones de entrada y carga |
| saveOptions | LowCodeSaveOptions | Opciones de salida y guardado |
| openPassword | String | Contraseña para el cifrado del archivo |
| writePassword | String | Contraseña para la protección de la modificación de la hoja de cálculo |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class SpreadsheetLockerMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            
            // Procesa la hoja de cálculo con contraseñas de bloqueo/desbloqueo
            SpreadsheetLocker.Process(
                new LowCodeLoadOptions() { InputFile = "input.xlsx" },
                new LowCodeSaveOptions() 
                { 
                    OutputFile = "output_locked.xlsx" 
                }, 
                "123456", 
                "234567");
        }
    }
}
```

### Ver también

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, string, string, string, ProtectionType) {#process_2}

Bloquea el archivo de hoja de cálculo con la configuración especificada.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    string openPassword, string writePassword, string workbookPassword, ProtectionType workbookType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Opciones de entrada y carga |
| saveOptions | LowCodeSaveOptions | Opciones de salida y guardado |
| openPassword | String | Contraseña para el cifrado del archivo |
| writePassword | String | Contraseña para la protección de la modificación de la hoja de cálculo |
| workbookPassword | String | Contraseña para la protección del libro de trabajo |
| workbookType | ProtectionType | Tipo de protección para proteger el libro de trabajo |

### Ver también

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeProtectionProvider) {#process}

Bloquea el archivo de hoja de cálculo con la configuración especificada.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    AbstractLowCodeProtectionProvider provider)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Opciones de entrada y carga |
| saveOptions | LowCodeSaveOptions | Opciones de salida y guardado |
| provider | AbstractLowCodeProtectionProvider | Implementación para proporcionar configuraciones de protección |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetLockerMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo1
    {
        public static void Run()
        {
           
            // Preparar LowCodeLoadOptions
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "input.xlsx";

            // Preparar LowCodeSaveOptions
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            saveOptions.OutputFile = "output.xlsx";

            // Crear un proveedor de protección personalizado
            CustomProtectionProvider provider = new CustomProtectionProvider();

            try
            {
                // Llamar al método estático Process con los parámetros especificados
                SpreadsheetLocker.Process(loadOptions, saveOptions, provider);

                Console.WriteLine("Spreadsheet processed and protected successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error processing spreadsheet: {ex.Message}");
            }

        }

        private class CustomProtectionProvider : AbstractLowCodeProtectionProvider
        {
            public override string GetOpenPassword()
            {
                return "open123";
            }

            public override string GetWritePassword()
            {
                return "write123";
            }

            public override string GetWorkbookPassword()
            {
                return "workbook123";
            }

            public override ProtectionType GetWorkbookProtectionType()
            {
                return ProtectionType.All;
            }
        }
    }
}
```

### Ver también

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeProtectionProvider](../../abstractlowcodeprotectionprovider/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


