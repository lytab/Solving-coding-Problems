=> solution using a post option with adding in formdata _method , PUT or PATCH
```
var formdata=new FormData();
// adding _method field with value PUT or PATCH
formdata.append('_method',"PUT"); or formdata.append('_method',"PATCH");
formdata.append('field1',val1);
formdata.append('field2',val2);
formdata.append('field3',val3);
.
.
.
formdata.append('fieldn',valn);
//using post option instead of put or patch
axios.post('api/url/'+id,formdata).then(response=>{
 // code
}).catch(error=>{
// catch errors
})
```
