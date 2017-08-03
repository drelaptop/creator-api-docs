## `NodePool` Class



Module: [cc](../modules/cc.md)




cc.NodePool 是用于管理节点对象的对象缓存池。<br/>
它可以帮助您提高游戏性能，适用于优化对象的反复创建和销毁<br/>
以前 cocos2d-x 中的 cc.pool 和新的节点事件注册系统不兼容，因此请使用 cc.NodePool 来代替。

新的 NodePool 需要实例化之后才能使用，每种不同的节点对象池需要一个不同的对象池实例，这里的种类对应于游戏中的节点设计，一个 prefab 相当于一个种类的节点。<br/>
在创建缓冲池时，可以传入一个包含 unuse, reuse 函数的组件类型用于节点的回收和复用逻辑。<br/>

一些常见的用例是：<br/>
     1.在游戏中的子弹（死亡很快，频繁创建，对其他对象无副作用）<br/>
     2.糖果粉碎传奇中的木块（频繁创建）。
     等等....

### Index

##### Properties

  - [`poolHandlerComp`](#poolhandlercomp) `Function|String` 缓冲池处理组件，用于节点的回收和复用逻辑，这个属性可以是组件类名或组件的构造函数。



##### Methods

  - [`constructor`](#constructor) 使用构造函数来创建一个节点专用的对象池，您可以传递一个组件类型或名称，用于处理节点回收和复用时的事件逻辑。
  - [`size`](#size) 获取当前缓冲池的可用对象数量
  - [`clear`](#clear) 销毁对象池中缓存的所有节点
  - [`put`](#put) 向缓冲池中存入一个不再需要的节点对象。
这个函数会自动将目标节点从父节点上移除，但是不会进行 cleanup 操作。
这个函数会调用 poolHandlerComp 的 unuse 函数，如果组件和函数都存在的话。
  - [`get`](#get) 获取对象池中的对象，如果对象池没有可用对象，则返回空。
这个函数会调用 poolHandlerComp 的 reuse 函数，如果组件和函数都存在的话。



### Details


#### Properties


##### poolHandlerComp

> 缓冲池处理组件，用于节点的回收和复用逻辑，这个属性可以是组件类名或组件的构造函数。

| meta | description |
|------|-------------|
| Type | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Function" class="crosslink external" target="_blank">Function</a> | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> |
| Defined | [https:/github.com/cocos-creator/engine/blob/master/extensions/ccpool/CCNodePool.js:75](https:/github.com/cocos-creator/engine/blob/master/extensions/ccpool/CCNodePool.js#L75) |






<!-- Method Block -->
#### Methods


##### constructor

使用构造函数来创建一个节点专用的对象池，您可以传递一个组件类型或名称，用于处理节点回收和复用时的事件逻辑。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/extensions/ccpool/CCNodePool.js:56](https:/github.com/cocos-creator/engine/blob/master/extensions/ccpool/CCNodePool.js#L56) |

###### Parameters
- poolHandlerComp <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Function" class="crosslink external" target="_blank">Function</a> | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> !#en The constructor or the class name of the component to control the unuse/reuse logic. !#zh 处理节点回收和复用事件逻辑的组件类型或名称。

##### Example

```js
properties: {
   template: cc.Prefab
 },
 onLoad () {
// MyTemplateHandler is a component with 'unuse' and 'reuse' to handle events when node is reused or recycled.
   this.myPool = new cc.NodePool('MyTemplateHandler');
 }
```

##### size

获取当前缓冲池的可用对象数量

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/extensions/ccpool/CCNodePool.js:87](https:/github.com/cocos-creator/engine/blob/master/extensions/ccpool/CCNodePool.js#L87) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> 



##### clear

销毁对象池中缓存的所有节点

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/extensions/ccpool/CCNodePool.js:97](https:/github.com/cocos-creator/engine/blob/master/extensions/ccpool/CCNodePool.js#L97) |



##### put

向缓冲池中存入一个不再需要的节点对象。
这个函数会自动将目标节点从父节点上移除，但是不会进行 cleanup 操作。
这个函数会调用 poolHandlerComp 的 unuse 函数，如果组件和函数都存在的话。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/extensions/ccpool/CCNodePool.js:110](https:/github.com/cocos-creator/engine/blob/master/extensions/ccpool/CCNodePool.js#L110) |

###### Parameters
- obj <a href="../classes/Node.html" class="crosslink">Node</a> 

##### Example

```js
let myNode = cc.instantiate(this.template);
  this.myPool.put(myNode);
```

##### get

获取对象池中的对象，如果对象池没有可用对象，则返回空。
这个函数会调用 poolHandlerComp 的 reuse 函数，如果组件和函数都存在的话。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/extensions/ccpool/CCNodePool.js:138](https:/github.com/cocos-creator/engine/blob/master/extensions/ccpool/CCNodePool.js#L138) |
| Return 		 | <a href="../classes/Node.html" class="crosslink">Node</a> | Null 

###### Parameters
- params Any !#en Params to pass to 'reuse' method in poolHandlerComp !#zh 向 poolHandlerComp 中的 'reuse' 函数传递的参数

##### Example

```js
let newNode = this.myPool.get();
```

