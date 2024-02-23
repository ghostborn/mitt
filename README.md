## mitt
一个小型的发布订阅模式js库

## Install
 --- 
`npm i mitt-jialp`

 ## Usage
  --- 
```javascript
 import mitt from 'mitt'
 
 const emitter = mitt()
 
 // listen to an event
 emitter.on('foo', e => console.log('foo', e) )
 
 // listen to all events
 emitter.on('*', (type, e) => console.log(type, e) )
 
 // fire an event
 emitter.emit('foo', { a: 'b' })
 
 // clearing all events
 emitter.all.clear()
 
 // working with handler references:
 function onFoo() {}
 emitter.on('foo', onFoo)   // listen
 emitter.off('foo', onFoo)  // unlisten
```
