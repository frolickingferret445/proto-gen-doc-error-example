# Protocol Documentation
<a name="top"/>

## Table of Contents

- [sample.proto](#sample.proto)
    - [Bar](#my.package.Bar)
    - [Foo](#my.package.Foo)
    - [GetBarRequest](#my.package.GetBarRequest)
    - [GetFooRequest](#my.package.GetFooRequest)



    - [MyService](#my.package.MyService)


- [Scalar Value Types](#scalar-value-types)



<a name="sample.proto"/>
<p align="right"><a href="#top">Top</a></p>

## sample.proto



<a name="my.package.Bar"/>

### Bar
Nothing to see here


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| bar | [string](#string) |  |  |






<a name="my.package.Foo"/>

### Foo
The same issue happens with messages.

multi-line descriptions are allowed for the top-level message


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| foo | [string](#string) |  | but

not

for

field |
| foo_count | [int32](#int32) |  | This field is not added to the table now. Lots of crazy pipes. |






<a name="my.package.GetBarRequest"/>

### GetBarRequest
Nothing to see here






<a name="my.package.GetFooRequest"/>

### GetFooRequest
Nothing to see here












<a name="my.package.MyService"/>

### MyService
This is a comment on a service.  It seems to work fine.

You can even skip lines like this.

or do fancy spacing like this:

     item1:     Description 1 goes here
     item2:         Description 2 goes here
     item3:        Description 3 goes here

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| GetFoo | [GetFooRequest](#my.package.GetFooRequest) | [Foo](#my.package.GetFooRequest) | However,

if you try to do the same thing with a nested rpc,

all of these random

pipes are generated and not all of the fields show up |
| GetBar | [GetBarRequest](#my.package.GetBarRequest) | [Bar](#my.package.GetBarRequest) | Then, a later rpc with a normal comment doesn&#39;t get added into the table. |





## Scalar Value Types

| .proto Type | Notes | C++ Type | Java Type | Python Type |
| ----------- | ----- | -------- | --------- | ----------- |
| <a name="double" /> double |  | double | double | float |
| <a name="float" /> float |  | float | float | float |
| <a name="int32" /> int32 | Uses variable-length encoding. Inefficient for encoding negative numbers – if your field is likely to have negative values, use sint32 instead. | int32 | int | int |
| <a name="int64" /> int64 | Uses variable-length encoding. Inefficient for encoding negative numbers – if your field is likely to have negative values, use sint64 instead. | int64 | long | int/long |
| <a name="uint32" /> uint32 | Uses variable-length encoding. | uint32 | int | int/long |
| <a name="uint64" /> uint64 | Uses variable-length encoding. | uint64 | long | int/long |
| <a name="sint32" /> sint32 | Uses variable-length encoding. Signed int value. These more efficiently encode negative numbers than regular int32s. | int32 | int | int |
| <a name="sint64" /> sint64 | Uses variable-length encoding. Signed int value. These more efficiently encode negative numbers than regular int64s. | int64 | long | int/long |
| <a name="fixed32" /> fixed32 | Always four bytes. More efficient than uint32 if values are often greater than 2^28. | uint32 | int | int |
| <a name="fixed64" /> fixed64 | Always eight bytes. More efficient than uint64 if values are often greater than 2^56. | uint64 | long | int/long |
| <a name="sfixed32" /> sfixed32 | Always four bytes. | int32 | int | int |
| <a name="sfixed64" /> sfixed64 | Always eight bytes. | int64 | long | int/long |
| <a name="bool" /> bool |  | bool | boolean | boolean |
| <a name="string" /> string | A string must always contain UTF-8 encoded or 7-bit ASCII text. | string | String | str/unicode |
| <a name="bytes" /> bytes | May contain any arbitrary sequence of bytes. | string | ByteString | str |
