##DigitalSignature class
## DigitalSignature class
Signature in file.
The DigitalSignature type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self, certificate, comments, sign_time)`](/cells/python-net/aspose.cells.digitalsignatures/digitalsignature/__init__/#system.security.cryptography.x509certificates.x509certificate2-system.string-system.datetime) | Constructor of digitalSignature. Uses .Net implementation. |
| [`__init__(self, raw_data, password, comments, sign_time)`](/cells/python-net/aspose.cells.digitalsignatures/digitalsignature/__init__/#bytes-system.string-system.string-system.datetime) | Constructor of digitalSignature. Uses Bouncy Castle implementation. |
### Properties
| Property | Description |
| :- | :- |
| [certificate](/cells/python-net/aspose.cells.digitalsignatures/digitalsignature/certificate) | Certificate object that was used to sign the document. |
| [comments](/cells/python-net/aspose.cells.digitalsignatures/digitalsignature/comments) | The purpose to signature. |
| [sign_time](/cells/python-net/aspose.cells.digitalsignatures/digitalsignature/sign_time) | The time when the document was signed. |
| [id](/cells/python-net/aspose.cells.digitalsignatures/digitalsignature/id) | Specifies a GUID which can be cross-referenced with the GUID of the signature line stored in the document content.
| [text](/cells/python-net/aspose.cells.digitalsignatures/digitalsignature/text) | Specifies the text of actual signature in the digital signature.
| [image](/cells/python-net/aspose.cells.digitalsignatures/digitalsignature/image) | Specifies an image for the digital signature.
| [provider_id](/cells/python-net/aspose.cells.digitalsignatures/digitalsignature/provider_id) | Specifies the class ID of the signature provider.
| [is_valid](/cells/python-net/aspose.cells.digitalsignatures/digitalsignature/is_valid) | If this digital signature is valid and the document has not been tampered with,
| [x_ad_es_type](/cells/python-net/aspose.cells.digitalsignatures/digitalsignature/x_ad_es_type) | XAdES type.
### See Also
* module [`aspose.cells.digitalsignatures`](..)
