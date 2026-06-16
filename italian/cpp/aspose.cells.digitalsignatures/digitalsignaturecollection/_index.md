---
title: Aspose::Cells::DigitalSignatures::DigitalSignatureCollection class
linktitle: DigitalSignatureCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::DigitalSignatures::DigitalSignatureCollection class. Provides a collection of digital signatures attached to a document in C++.'
type: docs
weight: 200
url: /it/cpp/aspose.cells.digitalsignatures/digitalsignaturecollection/
---
## DigitalSignatureCollection class


Provides a collection of digital signatures attached to a document.

```cpp
class DigitalSignatureCollection
```

## Methods

| Method | Description |
| --- | --- |
| [Add(const DigitalSignature\& digitalSignature)](./add/) | Add one signature to [DigitalSignatureCollection](./). |
| [DigitalSignatureCollection()](./digitalsignaturecollection/) | The constructor of [DigitalSignatureCollection](./). |
| [DigitalSignatureCollection(DigitalSignatureCollection_Impl* impl)](./digitalsignaturecollection/) | Constructs from an implementation object. |
| [DigitalSignatureCollection(const DigitalSignatureCollection\& src)](./digitalsignaturecollection/) | Copy constructor. |
| [GetEnumerator()](./getenumerator/) | Get the enumerator for [DigitalSignatureCollection](./), this enumerator allows iteration over the collection. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const DigitalSignatureCollection\& src)](./operator_asm/) | operator= |
| [~DigitalSignatureCollection()](./~digitalsignaturecollection/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Il seguente esempio mostra come convalidare la firma digitale.
//cartella di lavoro da un file sorgente firmato
Workbook signedWorkbook(u"signedFile.xlsx");
//wb.IsDigitallySigned è true quando la cartella di lavoro è già firmata.
std::cout<<signedWorkbook.IsDigitallySigned() << std::endl;
//ottieni la collezione digitalSignature dalla cartella di lavoro
DigitalSignatureCollection existingDsc = signedWorkbook.GetDigitalSignature();
Enumerator<DigitalSignature> en = existingDsc.GetEnumerator();
while (en.MoveNext())
{
    DigitalSignature existingDs = (DigitalSignature)en.GetCurrent();
    std::cout << "existingDs.Comments : " << existingDs.GetComments().ToUtf8() << std::endl;
    Date dt = existingDs.GetSignTime();
    std::cout << "existingDs.SignTime : " << dt.year << "-" << dt.month << "-" << dt.day << " " << dt.hour << ":" << dt.minute << ":" << dt.second << std::endl;
    std::cout << "existingDs.IsValid = " << (existingDs.IsValid() ? "True" : "False") << std::endl;
}

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::DigitalSignatures](../)
* Library [Aspose.Cells for C++](../../)
