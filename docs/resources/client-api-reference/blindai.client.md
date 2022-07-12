<!-- markdownlint-disable -->

<a href="../../../../blindai/client/blindai/client#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

# <kbd>module</kbd> `blindai.client`




**Global Variables**
---------------
- **app_version**
- **CONNECTION_TIMEOUT**


---

<a href="../../../../blindai/client/blindai/client/ModelDatumType"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

## <kbd>class</kbd> `ModelDatumType`
An enumeration. 





---

<a href="../../../../blindai/client/blindai/client/SignedResponse#L89"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

## <kbd>class</kbd> `SignedResponse`







---

<a href="../../../../blindai/client/blindai/client/as_bytes#L114"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `as_bytes`

```python
as_bytes() → bytes
```

Save the response as bytes. The response can later be loaded with: ```py
res = SignedResponse()
res.load_from_bytes(data)
``` 



**Returns:**
 
 - <b>`bytes`</b>:  The data. 

---

<a href="../../../../blindai/client/blindai/client/is_signed#L97"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `is_signed`

```python
is_signed() → bool
```





---

<a href="../../../../blindai/client/blindai/client/is_simulation_mode#L94"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `is_simulation_mode`

```python
is_simulation_mode() → bool
```





---

<a href="../../../../blindai/client/blindai/client/load_from_bytes#L140"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `load_from_bytes`

```python
load_from_bytes(b: bytes)
```

Load the response from bytes. 



**Args:**
 
 - <b>`b`</b> (bytes):  The data. 

---

<a href="../../../../blindai/client/blindai/client/load_from_file#L131"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `load_from_file`

```python
load_from_file(path: str)
```

Load the response from a file. 



**Args:**
 
 - <b>`path`</b> (str):  Path of the file. 

---

<a href="../../../../blindai/client/blindai/client/save_to_file#L100"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `save_to_file`

```python
save_to_file(path: str)
```

Save the response to a file. The response can later be loaded with: ```py
res = SignedResponse()
res.load_from_file(path)
``` 



**Args:**
 
 - <b>`path`</b> (str):  Path of the file. 


---

<a href="../../../../blindai/client/blindai/client/UploadModelResponse#L156"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

## <kbd>class</kbd> `UploadModelResponse`







---

<a href="../../../../blindai/client/blindai/client/as_bytes#L114"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `as_bytes`

```python
as_bytes() → bytes
```

Save the response as bytes. The response can later be loaded with: ```py
res = SignedResponse()
res.load_from_bytes(data)
``` 



**Returns:**
 
 - <b>`bytes`</b>:  The data. 

---

<a href="../../../../blindai/client/blindai/client/is_signed#L97"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `is_signed`

```python
is_signed() → bool
```





---

<a href="../../../../blindai/client/blindai/client/is_simulation_mode#L94"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `is_simulation_mode`

```python
is_simulation_mode() → bool
```





---

<a href="../../../../blindai/client/blindai/client/load_from_bytes#L140"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `load_from_bytes`

```python
load_from_bytes(b: bytes)
```

Load the response from bytes. 



**Args:**
 
 - <b>`b`</b> (bytes):  The data. 

---

<a href="../../../../blindai/client/blindai/client/load_from_file#L131"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `load_from_file`

```python
load_from_file(path: str)
```

Load the response from a file. 



**Args:**
 
 - <b>`path`</b> (str):  Path of the file. 

---

<a href="../../../../blindai/client/blindai/client/save_to_file#L100"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `save_to_file`

```python
save_to_file(path: str)
```

Save the response to a file. The response can later be loaded with: ```py
res = SignedResponse()
res.load_from_file(path)
``` 



**Args:**
 
 - <b>`path`</b> (str):  Path of the file. 

---

<a href="../../../../blindai/client/blindai/client/validate#L157"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `validate`

```python
validate(
    model_hash: bytes,
    policy_file: Optional[str] = None,
    policy: Optional[Policy] = None,
    validate_quote: bool = True,
    enclave_signing_key: Optional[bytes] = None,
    allow_simulation_mode: bool = False
)
```

Validates whether this response is valid. This is used for responses you have saved as bytes or in a file. This will raise an error if the response is not signed or if it is not valid. 



**Args:**
 
 - <b>`model_hash`</b> (bytes):  Hash of the model to verify against. 
 - <b>`policy_file`</b> (Optional[str], optional):  Path to the policy file. Defaults to None. 
 - <b>`policy`</b> (Optional[Policy], optional):  Policy to use. Use `policy_file` to load from a file directly. Defaults to None. 
 - <b>`validate_quote`</b> (bool, optional):  Whether or not the attestation should be validated too. Defaults to True. 
 - <b>`enclave_signing_key`</b> (Optional[bytes], optional):  Enclave signing key in case the attestation should not be validated. Defaults to None. 
 - <b>`allow_simulation_mode`</b> (bool, optional):  Whether or not simulation mode responses should be accepted. Defaults to False. 



**Raises:**
 
 - <b>`AttestationError`</b>:  Attestation is invalid. 
 - <b>`SignatureError`</b>:  Signed response is invalid. 
 - <b>`FileNotFoundError`</b>:  Will be raised if the policy file is not found. 


---

<a href="../../../../blindai/client/blindai/client/RunModelResponse#L211"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

## <kbd>class</kbd> `RunModelResponse`







---

<a href="../../../../blindai/client/blindai/client/as_bytes#L114"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `as_bytes`

```python
as_bytes() → bytes
```

Save the response as bytes. The response can later be loaded with: ```py
res = SignedResponse()
res.load_from_bytes(data)
``` 



**Returns:**
 
 - <b>`bytes`</b>:  The data. 

---

<a href="../../../../blindai/client/blindai/client/is_signed#L97"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `is_signed`

```python
is_signed() → bool
```





---

<a href="../../../../blindai/client/blindai/client/is_simulation_mode#L94"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `is_simulation_mode`

```python
is_simulation_mode() → bool
```





---

<a href="../../../../blindai/client/blindai/client/load_from_bytes#L140"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `load_from_bytes`

```python
load_from_bytes(b: bytes)
```

Load the response from bytes. 



**Args:**
 
 - <b>`b`</b> (bytes):  The data. 

---

<a href="../../../../blindai/client/blindai/client/load_from_file#L131"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `load_from_file`

```python
load_from_file(path: str)
```

Load the response from a file. 



**Args:**
 
 - <b>`path`</b> (str):  Path of the file. 

---

<a href="../../../../blindai/client/blindai/client/save_to_file#L100"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `save_to_file`

```python
save_to_file(path: str)
```

Save the response to a file. The response can later be loaded with: ```py
res = SignedResponse()
res.load_from_file(path)
``` 



**Args:**
 
 - <b>`path`</b> (str):  Path of the file. 

---

<a href="../../../../blindai/client/blindai/client/validate#L214"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `validate`

```python
validate(
    data_list: List[Any],
    policy_file: Optional[str] = None,
    policy: Optional[Policy] = None,
    validate_quote: bool = True,
    enclave_signing_key: Optional[bytes] = None,
    allow_simulation_mode: bool = False
)
```

Validates whether this response is valid. This is used for responses you have saved as bytes or in a file. This will raise an error if the response is not signed or if it is not valid. 



**Args:**
 
 - <b>`data_list`</b> (List[Any]):  Input used to run the model, to validate against. 
 - <b>`policy_file`</b> (Optional[str], optional):  Path to the policy file. Defaults to None. 
 - <b>`policy`</b> (Optional[Policy], optional):  Policy to use. Use `policy_file` to load from a file directly. Defaults to None. 
 - <b>`validate_quote`</b> (bool, optional):  Whether or not the attestation should be validated too. Defaults to True. 
 - <b>`enclave_signing_key`</b> (Optional[bytes], optional):  Enclave signing key in case the attestation should not be validated. Defaults to None. 
 - <b>`allow_simulation_mode`</b> (bool, optional):  Whether or not simulation mode responses should be accepted. Defaults to False. 



**Raises:**
 
 - <b>`AttestationError`</b>:  Attestation is invalid. 
 - <b>`SignatureError`</b>:  Signed response is invalid. 
 - <b>`FileNotFoundError`</b>:  Will be raised if the policy file is not found. 


---

<a href="../../../../blindai/client/blindai/client/BlindAiClient#L273"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

## <kbd>class</kbd> `BlindAiClient`




<a href="../../../../blindai/client/blindai/client/__init__#L284"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `__init__`

```python
__init__(debug_mode=False)
```








---

<a href="../../../../blindai/client/blindai/client/close_connection#L570"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `close_connection`

```python
close_connection()
```

Close the connection between the client and the inference server. 

---

<a href="../../../../blindai/client/blindai/client/connect_server#L310"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `connect_server`

```python
connect_server(
    addr: str,
    server_name: str = 'blindai-srv',
    policy: Optional[str] = None,
    certificate: Optional[str] = None,
    simulation: bool = False,
    untrusted_port: int = 50052,
    attested_port: int = 50051
)
```

Connect to the server with the specified parameters. You will have to specify here the expected policy (server identity, configuration...) and the server TLS certificate, if you are using the hardware mode. 

If you're using the simulation mode, you don't need to provide a policy and certificate, but please keep in mind that this mode should NEVER be used in production as it doesn't have most of the security provided by the hardware mode. 



**Args:**
 
 - <b>`addr`</b> (str):  The address of BlindAI server you want to reach. 
 - <b>`server_name`</b> (str, optional):  Contains the CN expected by the server TLS certificate. Defaults to "blindai-srv". 
 - <b>`policy`</b> (Optional[str], optional):  Path to the toml file describing the policy of the server.  Generated in the server side. Defaults to None. 
 - <b>`certificate`</b> (Optional[str], optional):  Path to the public key of the untrusted inference server.  Generated in the server side. Defaults to None. 
 - <b>`simulation`</b> (bool, optional):  Connect to the server in simulation mode.  If set to True, the args policy and certificate will be ignored. Defaults to False. 
 - <b>`untrusted_port`</b> (int, optional):  Untrusted connection server port. Defaults to 50052. 
 - <b>`attested_port`</b> (int, optional):  Attested connection server port. Defaults to 50051. 



**Raises:**
 
 - <b>`AttestationError`</b>:  Will be raised in case the policy doesn't match the  server identity and configuration, or if te attestation is invalid. 
 - <b>`ConnectionError`</b>:  will be raised if the connection with the server fails. 
 - <b>`VersionError`</b>:  Will be raised if the version of the server is not supported by the client. 
 - <b>`FileNotFoundError`</b>:  will be raised if the policy file, or the certificate file is not  found (in Hardware mode). 

---

<a href="../../../../blindai/client/blindai/client/is_connected#L302"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `is_connected`

```python
is_connected() → bool
```





---

<a href="../../../../blindai/client/blindai/client/run_model#L512"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `run_model`

```python
run_model(data_list: List[Any], sign: bool = False) → RunModelResponse
```

Send data to the server to make a secure inference. 

The data provided must be in a list, as the tensor will be rebuilt inside the server. 



**Args:**
 
 - <b>`data_list`</b> (List[Any]):  The input data. It must be an array of numbers of the same type dtype specified in `upload_model`. 
 - <b>`sign`</b> (bool, optional):  Get signed responses from the server or not. Defaults to False. 



**Raises:**
 
 - <b>`ConnectionError`</b>:  Will be raised if the client is not connected. 
 - <b>`SignatureError`</b>:  Will be raised if the response signature is invalid 



**Returns:**
 
 - <b>`RunModelResponse`</b>:  The response object. 

---

<a href="../../../../blindai/client/blindai/client/upload_model#L439"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `upload_model`

```python
upload_model(
    model: str,
    shape: Tuple = None,
    dtype: ModelDatumType = <ModelDatumType.F32: 0>,
    dtype_out: ModelDatumType = <ModelDatumType.F32: 0>,
    sign: bool = False
) → UploadModelResponse
```

Upload an inference model to the server. The provided model needs to be in the Onnx format. 



**Args:**
 
 - <b>`model`</b> (str):  Path to Onnx model file. 
 - <b>`shape`</b> (Tuple, optional):  The shape of the model input. Defaults to None. 
 - <b>`dtype`</b> (ModelDatumType, optional):  The type of the model input data (f32 by default). Defaults to ModelDatumType.F32. 
 - <b>`dtype_out`</b> (ModelDatumType, optional):  The type of the model output data (f32 by default). Defaults to ModelDatumType.F32. 
 - <b>`sign`</b> (bool, optional):  Get signed responses from the server or not. Defaults to False. 



**Raises:**
 
 - <b>`ConnectionError`</b>:  Will be raised if the client is not connected. 
 - <b>`FileNotFoundError`</b>:  Will be raised if the model file is not found. 
 - <b>`SignatureError`</b>:  Will be raised if the response signature is invalid. 



**Returns:**
 
 - <b>`UploadModelResponse`</b>:  The response object. 




---

_This file was automatically generated via [lazydocs](https://github.com/ml-tooling/lazydocs)._
