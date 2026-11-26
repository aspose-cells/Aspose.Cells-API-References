---
title: "Класс DigitalSignatureCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.DigitalSignatures.DigitalSignatureCollection. Предоставляет коллекцию цифровых подписей, прикреплённых к документу"
type: docs
url: /ru/net/aspose.cells.digitalsignatures/digitalsignaturecollection/
---
## DigitalSignatureCollection class

Предоставляет коллекцию цифровых подписей, прикреплённых к документу.

```csharp
public class DigitalSignatureCollection : IEnumerable
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [DigitalSignatureCollection](digitalsignaturecollection/)() | Конструктор класса DigitalSignatureCollection. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.digitalsignatures/digitalsignaturecollection/add/)(DigitalSignature) | Добавить одну подпись в DigitalSignatureCollection. |
| [GetEnumerator](../../aspose.cells.digitalsignatures/digitalsignaturecollection/getenumerator/)() | Получить перечислитель для DigitalSignatureCollection, этот перечислитель позволяет выполнять итерацию по коллекции. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Security.Cryptography.X509Certificates;

    public class DigitalSignatureCollectionDemo
    {
        public static void DigitalSignatureCollectionExample()
        {
            // Загрузить книгу из подписанного исходного файла.
            Workbook signedWorkbook = new Workbook(@"DigitalSignatureCollection_original.xlsx");

            // Проверить, подписана ли книга цифровой подписью
            Console.WriteLine("Is the workbook digitally signed? " + signedWorkbook.IsDigitallySigned);

            // Получить коллекцию цифровых подписей из книги.
            DigitalSignatureCollection existingDsc = signedWorkbook.GetDigitalSignature();

            if (existingDsc != null)
            {
                // Итерировать цифровые подписи в коллекции.
                foreach (DigitalSignature existingDs in existingDsc)
                {
                    Console.WriteLine("Comments: " + existingDs.Comments);
                    Console.WriteLine("Sign Time: " + existingDs.SignTime);
                    Console.WriteLine("Is Valid: " + existingDs.IsValid);
                }

                // Создать новую цифровую подпись.
                X509Certificate2 certificate = new X509Certificate2("path_to_certificate.pfx", "password");
                DigitalSignature newSignature = new DigitalSignature(certificate, "New signature comment", DateTime.Now);

                // Добавить новую цифровую подпись в коллекцию.
                existingDsc.Add(newSignature);
            }     
            

            // Сохранить книгу с новой цифровой подписью.
            signedWorkbook.Save("DigitalSignatureCollectionExample.xlsx");
            signedWorkbook.Save("DigitalSignatureCollectionExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


