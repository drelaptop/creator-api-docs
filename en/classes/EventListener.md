## `EventListener` Class



Module: [cc](../modules/cc.md)




<p>
    The base class of event listener.                                                                        <br/>
    If you need custom listener which with different callback, you need to inherit this class.               <br/>
    For instance, you could refer to EventListenerAcceleration, EventListenerKeyboard,                       <br/>
     EventListenerTouchOneByOne, EventListenerCustom.
</p>

### Index

##### Properties

  - [`UNKNOWN`](#unknown) `Number` The type code of unknown event listener.
  - [`KEYBOARD`](#keyboard) `Number` The type code of keyboard event listener.
  - [`ACCELERATION`](#acceleration) `Number` The type code of acceleration event listener.



##### Methods

  - [`constructor`](#constructor) Constructor
  - [`checkAvailable`](#checkavailable) Checks whether the listener is available.
  - [`clone`](#clone) Clones the listener, its subclasses have to override this method.
  - [`setEnabled`](#setenabled) Enables or disables the listener
  - [`isEnabled`](#isenabled) Checks whether the listener is enabled
  - [`create`](#create) Create a EventListener object with configuration including the event type, handlers and other parameters.
In handlers, this refer to the event listener object itself.
You can also pass custom parameters in the configuration object,
all custom parameters will be polyfilled into the event listener object and can be accessed in handlers.



### Details


#### Properties


##### UNKNOWN

> The type code of unknown event listener.

| meta | description |
|------|-------------|
| Type | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> |
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/event-manager/CCEventListener.js:252](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/event-manager/CCEventListener.js#L252) |



##### KEYBOARD

> The type code of keyboard event listener.

| meta | description |
|------|-------------|
| Type | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> |
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/event-manager/CCEventListener.js:276](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/event-manager/CCEventListener.js#L276) |



##### ACCELERATION

> The type code of acceleration event listener.

| meta | description |
|------|-------------|
| Type | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> |
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/event-manager/CCEventListener.js:292](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/event-manager/CCEventListener.js#L292) |






<!-- Method Block -->
#### Methods


##### constructor

Constructor

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/event-manager/CCEventListener.js:44](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/event-manager/CCEventListener.js#L44) |

###### Parameters
- type <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> 
- listenerID <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> 
- callback <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> 


##### checkAvailable

Checks whether the listener is available.

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/event-manager/CCEventListener.js:173](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/event-manager/CCEventListener.js#L173) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Boolean" class="crosslink external" target="_blank">Boolean</a> 



##### clone

Clones the listener, its subclasses have to override this method.

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/event-manager/CCEventListener.js:183](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/event-manager/CCEventListener.js#L183) |
| Return 		 | <a href="../classes/EventListener.html" class="crosslink">EventListener</a> 



##### setEnabled

Enables or disables the listener

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/event-manager/CCEventListener.js:193](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/event-manager/CCEventListener.js#L193) |

###### Parameters
- enabled <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Boolean" class="crosslink external" target="_blank">Boolean</a> 


##### isEnabled

Checks whether the listener is enabled

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/event-manager/CCEventListener.js:207](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/event-manager/CCEventListener.js#L207) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Boolean" class="crosslink external" target="_blank">Boolean</a> 



##### create

Create a EventListener object with configuration including the event type, handlers and other parameters.
In handlers, this refer to the event listener object itself.
You can also pass custom parameters in the configuration object,
all custom parameters will be polyfilled into the event listener object and can be accessed in handlers.

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/event-manager/CCEventListener.js:453](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/event-manager/CCEventListener.js#L453) |
| Return 		 | <a href="../classes/EventListener.html" class="crosslink">EventListener</a> 

###### Parameters
- argObj <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Object" class="crosslink external" target="_blank">Object</a> a json object

##### Example

```Not found for the example path: utils/api/engine/docs/cocos2d/core/event-manager/CCEventListener/create.js

