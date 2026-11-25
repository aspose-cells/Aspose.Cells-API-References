---
title: "OleObject.SetNativeSourceFullName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo OleObject. Imposta il nome completo del file sorgente nativo ole con percorso"
type: docs
url: /it/net/aspose.cells.drawing/oleobject/setnativesourcefullname/
---
## OleObject.SetNativeSourceFullName method

Imposta il nome completo del file sorgente nativo ole con percorso.

```csharp
public void SetNativeSourceFullName(string sourceFullName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceFullName | String | Il nome completo del file sorgente nativo ole |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class OleObjectMethodSetNativeSourceFullNameWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un OleObject al foglio di lavoro
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]); // Changed to empty byte array
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // Chiama il metodo SetNativeSourceFullName con un parametro stringa
                oleObject.SetNativeSourceFullName(@"C:\temp\updated_test.xlsx");
                
                Console.WriteLine("SetNativeSourceFullName method executed successfully with parameter: C:\\temp\\updated_test.xlsx");
                
                // Visualizza l'effetto controllando la proprietà ObjectSourceFullName
                Console.WriteLine($"OleObject's source is now: {oleObject.ObjectSourceFullName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetNativeSourceFullName method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("OleObjectMethodSetNativeSourceFullNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


