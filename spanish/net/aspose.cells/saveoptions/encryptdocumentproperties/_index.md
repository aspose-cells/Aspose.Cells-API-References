---
title: "SaveOptions.EncryptDocumentProperties"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SaveOptions. Indica si se encriptan las propiedades del documento al guardar como archivo .xls. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells/saveoptions/encryptdocumentproperties/
---
## SaveOptions.EncryptDocumentProperties property

Indica si se encriptan las propiedades del documento al guardar como archivo .xls. El valor predeterminado es verdadero.

```csharp
public bool EncryptDocumentProperties { get; set; }
```

### Observaciones

Solo para archivos .xls, .xlsx, .xlsb y .xlsm.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyEncryptDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer algunas propiedades del documento
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Document";
            
            // Establecer protección con contraseña
            workbook.Settings.Password = "password123";
            
            // Guardar con EncryptDocumentProperties = true (predeterminado)
            XlsSaveOptions saveOptions1 = new XlsSaveOptions();
            saveOptions1.EncryptDocumentProperties = true;
            workbook.Save("encrypted_properties.xls", saveOptions1);
            
            // Guardar con EncryptDocumentProperties = false
            XlsSaveOptions saveOptions2 = new XlsSaveOptions();
            saveOptions2.EncryptDocumentProperties = false;
            workbook.Save("unencrypted_properties.xls", saveOptions2);
            
            // Verificar cargando nuevamente
            Console.WriteLine("Files saved. Try opening them to see the difference in property encryption.");
        }
    }
}
```

### Ver también

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


