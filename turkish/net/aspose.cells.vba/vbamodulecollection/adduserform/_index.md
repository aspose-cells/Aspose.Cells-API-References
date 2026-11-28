---
title: "VbaModuleCollection.AddUserForm"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaModuleCollection yöntemi. Kullanıcı formunu VBA Project'e ekler"
type: docs
url: /tr/net/aspose.cells.vba/vbamodulecollection/adduserform/
---
## VbaModuleCollection.AddUserForm method

Kullanıcı formunu VBA Projesine ekle.

```csharp
public int AddUserForm(string name, string codes, byte[] designerStorage)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Kullanıcı formunun adı |
| kodlar | String | Kullanıcı formu için kodlar |
| designerStorage | Byte[] | kullanıcı formu ile ilgili tasarım ayarı |

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // VBA projesine eriş
            VbaProject vbaProject = workbook.VbaProject;
            VbaModuleCollection vbaModules = vbaProject.Modules;

            // AddUserForm için parametreleri hazırlayın
            string formName = "UserForm1";
            string formCode = 
                "Private Sub CommandButton1_Click()\n" +
                "    MsgBox \"Hello from UserForm!\"\n" +
                "End Sub";
            
            // Basit bir tasarımcı depolama oluşturun (bu normalde .frx ikili verisi olur)
            byte[] designerStorage = new byte[] { 0x00, 0x01, 0x02, 0x03 };

            try
            {
                // AddUserForm'u (String, String, Byte[]) parametreleriyle çağırın
                int moduleIndex = vbaModules.AddUserForm(formName, formCode, designerStorage);
                
                Console.WriteLine($"UserForm added successfully at index: {moduleIndex}");
                Console.WriteLine($"Total VBA modules: {vbaModules.Count}");

                // VBA proje değişikliklerini görmek için çalışma kitabını kaydedin
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

### Ayrıca Bakınız

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


