# keep

```
import 'keep.js'

var k = keep('https://hashsan.github.io/counter');
var name = 'foo.txt'
var text = await k.get(name)
text = text +'\nnew line';
await k.set(name,text)

var ary = await k.list()
/*
[
{
  file:'foo.txt',
  title:'xyzaaaa',
  date:'2024-04-25 14:55',
  order: 145322  //~~((Date.now() - new Date(date).getTime())/(60*1000))
},
{
}

]
*/


```
