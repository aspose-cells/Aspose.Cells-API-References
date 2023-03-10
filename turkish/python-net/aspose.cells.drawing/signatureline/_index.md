---
title: SignatureLine sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 640
url: /tr/python-net/aspose.cells.drawing/signatureline/
is_root: false
---
##  SignatureLine sınıfı
İmza satırını temsil eder.



SignatureLine türü aşağıdaki üyeleri gösterir:

###  İnşaatçılar
| Yapıcı| Tanım|
| :- | :- |
| [SignatureLine()](/cells/tr/python-net/aspose.cells.drawing/signatureline/__init__/#) | SignatureLine'ın yeni bir örneğini oluşturur|


###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [id](/cells/tr/python-net/aspose.cells.drawing/signatureline/id) | Bu imza satırı için tanımlayıcıyı alır veya ayarlar.|
| [provider_id](/cells/tr/python-net/aspose.cells.drawing/signatureline/provider_id) | İmza sağlayıcının kimliğini alır ve ayarlar.|
| [signer](/cells/tr/python-net/aspose.cells.drawing/signatureline/signer) | İmzalayanı alır ve ayarlar.|
| [title](/cells/tr/python-net/aspose.cells.drawing/signatureline/title) | Şarkıcı unvanını alır ve ayarlar.|
| [email](/cells/tr/python-net/aspose.cells.drawing/signatureline/email) | Şarkıcının e-postasını alır ve ayarlar.|
| [is_line](/cells/tr/python-net/aspose.cells.drawing/signatureline/is_line) | İmza satırı olup olmadığını gösterir.|
| [allow_comments](/cells/tr/python-net/aspose.cells.drawing/signatureline/allow_comments) | Yorumların iliştirilip eklenemeyeceğini belirtir.|
| [show_signed_date](/cells/tr/python-net/aspose.cells.drawing/signatureline/show_signed_date) | İmza tarihini gösterip göstermediğini gösterir.|
| [instructions](/cells/tr/python-net/aspose.cells.drawing/signatureline/instructions) | İmzalama anında kullanıcıya gösterilen metni alır ve ayarlar.|



###  Örnek

```python
from aspose.cells import Workbook
from aspose.cells.drawing import SignatureLine

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# Adding a picture
imgIndex = worksheet.pictures.add(1, 1, "sample.png")
pic = worksheet.pictures[imgIndex]
#  Create signature line object
s = SignatureLine()
s.signer = "Simon Zhao"
s.title = "Development Lead"
s.email = "Simon.Zhao@aspose.com"
#  Assign the signature line object to Picture.SignatureLine property
pic.signature_line = s
# do your business
# Save the excel file.
workbook.save("result.xlsx")

```

###  Ayrıca bakınız
* modül [aspose.cells.drawing](..)
