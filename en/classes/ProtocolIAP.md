## `ProtocolIAP` Class

Extends [`PluginProtocol`](PluginProtocol.md)


Module: [anysdk](../modules/anysdk.md)




IAP protocol

### Index



##### Methods

  - [`payForProduct`](#payforproduct) pay interface
  - [`getOrderId`](#getorderid) get order ID
  - [`resetPayState`](#resetpaystate) reset the pay status
  - [`getPluginId`](#getpluginid) get plugin ID
  - [`setListener`](#setlistener) set listener
  - [`getListener`](#getlistener) get listener
  - [`isFunctionSupported`](#isfunctionsupported) Check whether the function is supported
  - [`getPluginName`](#getpluginname) get plugin name
  - [`getPluginVersion`](#getpluginversion) get plugin version
  - [`getSDKVersion`](#getsdkversion) get SDK version
  - [`callFuncWithParam`](#callfuncwithparam) void methods for reflections with parameter
  - [`callStringFuncWithParam`](#callstringfuncwithparam) String methods for reflections with parameter
  - [`callIntFuncWithParam`](#callintfuncwithparam) int methods for reflections with parameter
  - [`callBoolFuncWithParam`](#callboolfuncwithparam) boolean methods for reflections with parameter
  - [`callFloatFuncWithParam`](#callfloatfuncwithparam) float methods for reflections with parameter



### Details




<!-- Method Block -->
#### Methods


##### payForProduct

pay interface

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js:708](https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js#L708) |

###### Parameters
- info <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Object" class="crosslink external" target="_blank">Object</a> Type:map


##### getOrderId

get order ID

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js:719](https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js#L719) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 



##### resetPayState

reset the pay status

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js:731](https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js#L731) |



##### getPluginId

get plugin ID

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js:742](https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js#L742) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 



##### setListener

set listener

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js:754](https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js#L754) |

###### Parameters
- listener <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Function" class="crosslink external" target="_blank">Function</a> 
- target <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Object" class="crosslink external" target="_blank">Object</a> 


##### getListener

get listener

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js:766](https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js#L766) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Function" class="crosslink external" target="_blank">Function</a> 



##### isFunctionSupported

Check whether the function is supported

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js:327](https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js#L327) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Boolean" class="crosslink external" target="_blank">boolean</a> 

###### Parameters
- functionName <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 


##### getPluginName

get plugin name

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js:341](https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js#L341) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 



##### getPluginVersion

get plugin version

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js:353](https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js#L353) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 



##### getSDKVersion

get SDK version

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js:365](https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js#L365) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 



##### callFuncWithParam

void methods for reflections with parameter

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js:377](https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js#L377) |

###### Parameters
- funName <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 
- args <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Object" class="crosslink external" target="_blank">Object</a> | anysdk.PluginParam optional arguments


##### callStringFuncWithParam

String methods for reflections with parameter

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js:390](https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js#L390) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 

###### Parameters
- funName <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 
- args <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Object" class="crosslink external" target="_blank">Object</a> | anysdk.PluginParam optional arguments


##### callIntFuncWithParam

int methods for reflections with parameter

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js:405](https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js#L405) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> 

###### Parameters
- funName <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 
- args <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Object" class="crosslink external" target="_blank">Object</a> | anysdk.PluginParam optional arguments


##### callBoolFuncWithParam

boolean methods for reflections with parameter

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js:420](https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js#L420) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Boolean" class="crosslink external" target="_blank">boolean</a> 

###### Parameters
- funName <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 
- args <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Object" class="crosslink external" target="_blank">Object</a> | anysdk.PluginParam optional arguments


##### callFloatFuncWithParam

float methods for reflections with parameter

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js:435](https:/github.com/cocos-creator/engine/blob/master/extensions/anysdk/jsb_anysdk.js#L435) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> 

###### Parameters
- funName <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 
- args <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Object" class="crosslink external" target="_blank">Object</a> | anysdk.PluginParam optional arguments


