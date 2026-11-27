---
title: "VbaModuleCollection.AddUserForm"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaModuleCollection-metoden. Infoga användarformulär i VBA-projektet"
type: docs
url: /sv/net/aspose.cells.vba/vbamodulecollection/adduserform/
---
## VbaModuleCollection.AddUserForm method

Infoga användarformulär i VBA-projektet.

```csharp
public int AddUserForm(string name, string codes, byte[] designerStorage)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Namnet på användarformuläret |
| koder | String | Koderna för användarformuläret |
| designerStorage | Byte[] | designinställningen för användarformuläret |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;
    using System.IO;

    public class VbaModuleCollectionMethodAddUserFormWithStringStringByteDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till VBA-projektet
            VbaProject vbaProject = workbook.VbaProject;
            VbaModuleCollection vbaModules = vbaProject.Modules;

            // Förbered parametrar för AddUserForm
            string formName = "UserForm1";
            string formCode = 
                "Private Sub CommandButton1_Click()\n" +
                "    MsgBox \"Hello from UserForm!\"\n" +
                "End Sub";
            
            // Skapa en enkel designlagring (detta skulle normalt vara .frx-binärdata)
            byte[] designerStorage = new byte[] { 0x00, 0x01, 0x02, 0x03 };

            try
            {
                // Anropa AddUserForm med parametrarna (String, String, Byte[])
                int moduleIndex = vbaModules.AddUserForm(formName, formCode, designerStorage);
                
                Console.WriteLine($"UserForm added successfully at index: {moduleIndex}");
                Console.WriteLine($"Total VBA modules: {vbaModules.Count}");

                // Spara arbetsboken för att se förändringarna i VBA-projektet
                workbook.Save("AddUserFormDemo.xlsm", SaveFormat.Xlsm);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding UserForm: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


