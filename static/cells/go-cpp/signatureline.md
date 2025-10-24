##SignatureLine Class
'SignatureLine class. Encapsulates the object that represents signatureline in Go.'
## SignatureLine class
Represent the signature line.
```go
type SignatureLine struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewSignatureLine](./newsignatureline/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetId](./getid/) | Gets or sets identifier for this signature line. |
|[SetId](./setid/) | Gets or sets identifier for this signature line. |
|[GetProviderId](./getproviderid/) | Gets or sets the id of signature provider. |
|[SetProviderId](./setproviderid/) | Gets or sets the id of signature provider. |
|[GetSigner](./getsigner/) | Gets or sets the signer. |
|[SetSigner](./setsigner/) | Gets or sets the signer. |
|[GetTitle](./gettitle/) | Gets or sets the title of singer. |
|[SetTitle](./settitle/) | Gets or sets the title of singer. |
|[GetEmail](./getemail/) | Gets or sets the email of singer. |
|[SetEmail](./setemail/) | Gets or sets the email of singer. |
|[IsLine](./isline/) | Indicates whether it is a signature line. |
|[SetIsLine](./setisline/) | Indicates whether it is a signature line. |
|[GetAllowComments](./getallowcomments/) | Indicates whether comments could be attached. |
|[SetAllowComments](./setallowcomments/) | Indicates whether comments could be attached. |
|[GetShowSignedDate](./getshowsigneddate/) | Indicates whether show signed date. |
|[SetShowSignedDate](./setshowsigneddate/) | Indicates whether show signed date. |
|[GetInstructions](./getinstructions/) | Gets or sets the text shown to user at signing time. |
|[SetInstructions](./setinstructions/) | Gets or sets the text shown to user at signing time. |
|[GetSignatureLineType](./getsignaturelinetype/) | Gets or sets the signature type.Default - When the default value is set, the corresponding ProviderId value is fixed to {0000000000-0000-0000-0000-0000000000}.Stamp - When the value is Stamp, the corresponding ProviderId value is usually {000CD6A4-0000-0000-C000-000000000046}.Custom - When the value is Custom, the corresponding ProviderId value usually needs to be set by the user. it should be obtained from the documentation shipped with the provider. |
|[SetSignatureLineType](./setsignaturelinetype/) | Gets or sets the signature type.Default - When the default value is set, the corresponding ProviderId value is fixed to {0000000000-0000-0000-0000-0000000000}.Stamp - When the value is Stamp, the corresponding ProviderId value is usually {000CD6A4-0000-0000-C000-000000000046}.Custom - When the value is Custom, the corresponding ProviderId value usually needs to be set by the user. it should be obtained from the documentation shipped with the provider. |
