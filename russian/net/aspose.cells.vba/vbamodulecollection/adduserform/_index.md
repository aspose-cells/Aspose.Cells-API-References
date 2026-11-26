---
title: "VbaModuleCollection.AddUserForm"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод VbaModuleCollection. Вставляет пользовательскую форму в проект VBA"
type: docs
url: /ru/net/aspose.cells.vba/vbamodulecollection/adduserform/
---
## VbaModuleCollection.AddUserForm method

Вставить пользовательскую форму в проект VBA.

```csharp
public int AddUserForm(string name, string codes, byte[] designerStorage)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя пользовательской формы |
| коды | String | Коды для пользовательской формы |
| designerStorage | Byte[] | настройка дизайнера для пользовательской формы |

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Доступ к проекту VBA
            VbaProject vbaProject = workbook.VbaProject;
            VbaModuleCollection vbaModules = vbaProject.Modules;

            // Подготовьте параметры для AddUserForm
            string formName = "UserForm1";
            string formCode = 
                "Private Sub CommandButton1_Click()\n" +
                "    MsgBox \"Hello from UserForm!\"\n" +
                "End Sub";
            
            // Создайте простое хранилище дизайнера (обычно это двоичные данные .frx)
            byte[] designerStorage = new byte[] { 0x00, 0x01, 0x02, 0x03 };

            try
            {
                // Вызовите AddUserForm с параметрами (String, String, Byte[])
                int moduleIndex = vbaModules.AddUserForm(formName, formCode, designerStorage);
                
                Console.WriteLine($"UserForm added successfully at index: {moduleIndex}");
                Console.WriteLine($"Total VBA modules: {vbaModules.Count}");

                // Сохраните книгу, чтобы увидеть изменения проекта VBA
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

### См. также

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


