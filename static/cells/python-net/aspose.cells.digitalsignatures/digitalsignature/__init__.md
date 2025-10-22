##DigitalSignature constructor
## \_\_init\_\_(self, certificate, comments, sign_time) {#System.Security.Cryptography.X509Certificates.X509Certificate2-System.String-System.DateTime}
Constructor of digitalSignature. Uses .Net implementation.
```python
def __init__(self, certificate, comments, sign_time):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| certificate | System.Security.Cryptography.X509Certificates.X509Certificate2 | Certificate object that was used to sign the document. |
| comments | System.String | The purpose to signature. |
| sign_time | System.DateTime | The utc time when the document was signed. |
## \_\_init\_\_(self, raw_data, password, comments, sign_time) {#bytes-System.String-System.String-System.DateTime}
Constructor of digitalSignature. Uses Bouncy Castle implementation.
```python
def __init__(self, raw_data, password, comments, sign_time):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| raw_data | bytes | A byte array containing data from an X.509 certificate. |
| password | System.String | The password required to access the X.509 certificate data. |
| comments | System.String | The purpose to signature. |
| sign_time | System.DateTime | The utc time when the document was signed. |
### See Also
* module [`aspose.cells.digitalsignatures`](../../)
* class [`DigitalSignature`](/cells/python-net/aspose.cells.digitalsignatures/digitalsignature)
