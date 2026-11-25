---
title: "SaveOptions.EncryptDocumentProperties"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SaveOptions. Indica se crittografare le proprietà del documento durante il salvataggio come file .xls. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/saveoptions/encryptdocumentproperties/
---
## SaveOptions.EncryptDocumentProperties property

Indica se crittografare le proprietà del documento quando si salva come file .xls. Il valore predefinito è true.

```csharp
public bool EncryptDocumentProperties { get; set; }
```

### Osservazioni

Solo per file .xls, .xlsx, .xlsb e .xlsm.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyEncryptDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta alcune proprietà del documento
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Document";
            
            // Imposta protezione con password
            workbook.Settings.Password = "password123";
            
            // Salva con EncryptDocumentProperties = true (predefinito)
            XlsSaveOptions saveOptions1 = new XlsSaveOptions();
            saveOptions1.EncryptDocumentProperties = true;
            workbook.Save("encrypted_properties.xls", saveOptions1);
            
            // Salva con EncryptDocumentProperties = false
            XlsSaveOptions saveOptions2 = new XlsSaveOptions();
            saveOptions2.EncryptDocumentProperties = false;
            workbook.Save("unencrypted_properties.xls", saveOptions2);
            
            // Verifica ricaricando
            Console.WriteLine("Files saved. Try opening them to see the difference in property encryption.");
        }
    }
}
```

### Vedi anche

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


