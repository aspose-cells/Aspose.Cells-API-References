---
title: "VbaModuleCollection.AddUserForm"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método VbaModuleCollection. Insertar formulario de usuario en el proyecto VBA"
type: docs
url: /es/net/aspose.cells.vba/vbamodulecollection/adduserform/
---
## VbaModuleCollection.AddUserForm method

Insertar formulario de usuario en el proyecto VBA.

```csharp
public int AddUserForm(string name, string codes, byte[] designerStorage)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre del formulario de usuario |
| códigos | String | Los códigos del formulario de usuario |
| designerStorage | Byte[] | la configuración del diseñador del formulario de usuario |

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder al proyecto VBA
            VbaProject vbaProject = workbook.VbaProject;
            VbaModuleCollection vbaModules = vbaProject.Modules;

            // Preparar parámetros para AddUserForm
            string formName = "UserForm1";
            string formCode = 
                "Private Sub CommandButton1_Click()\n" +
                "    MsgBox \"Hello from UserForm!\"\n" +
                "End Sub";
            
            // Crear un almacenamiento de diseñador simple (esto normalmente sería los datos binarios .frx)
            byte[] designerStorage = new byte[] { 0x00, 0x01, 0x02, 0x03 };

            try
            {
                // Llamar a AddUserForm con parámetros (String, String, Byte[])
                int moduleIndex = vbaModules.AddUserForm(formName, formCode, designerStorage);
                
                Console.WriteLine($"UserForm added successfully at index: {moduleIndex}");
                Console.WriteLine($"Total VBA modules: {vbaModules.Count}");

                // Guarde el libro de trabajo para ver los cambios del proyecto VBA
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

### Ver también

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


