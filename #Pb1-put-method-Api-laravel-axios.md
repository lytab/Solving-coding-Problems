=> solution using a post option with adding in formdata _method , PUT or PATCH
```
var formdata=new FormData();
**formdata.append('_method',"PUT"); or formdata.append('_method',"PATCH");**
formdata.append('field1',val1);
formdata.append('field2',val2);
formdata.append('field3',val3);
.
.
.
formdata.append('fieldn',valn);

**axios._post_('api/url/'+id,formdata).then(response=>{**
 // code
}).catch(error=>{
// catch errors
})
```
