## `ResolutionPolicy` 类型



模块: [_decorator](../modules/_decorator.md)
父模块: [cc](../modules/cc.md)




<p>cc.ResolutionPolicy class is the root strategy class of scale strategy,
its main task is to maintain the compatibility with Cocos2d-x</p>

### 索引

##### 属性（properties）

  - [`EXACT_FIT`](#exactfit) `Number` The entire application is visible in the specified area without trying to preserve the original aspect ratio.<br/>
Distortion can occur, and the application may appear stretched or compressed.
  - [`NO_BORDER`](#noborder) `Number` The entire application fills the specified area, without distortion but possibly with some cropping,<br/>
while maintaining the original aspect ratio of the application.
  - [`SHOW_ALL`](#showall) `Number` The entire application is visible in the specified area without distortion while maintaining the original<br/>
aspect ratio of the application. Borders can appear on two sides of the application.
  - [`FIXED_HEIGHT`](#fixedheight) `Number` The application takes the height of the design resolution size and modifies the width of the internal<br/>
canvas so that it fits the aspect ratio of the device<br/>
no distortion will occur however you must make sure your application works on different<br/>
aspect ratios
  - [`FIXED_WIDTH`](#fixedwidth) `Number` The application takes the width of the design resolution size and modifies the height of the internal<br/>
canvas so that it fits the aspect ratio of the device<br/>
no distortion will occur however you must make sure your application works on different<br/>
aspect ratios
  - [`UNKNOWN`](#unknown) `Number` Unknow policy



##### 方法

  - [`constructor`](#constructor) 
  - [`preApply`](#preapply) Manipulation before applying the resolution policy
  - [`apply`](#apply) Function to apply this resolution policy
The return value is {scale: [scaleX, scaleY], viewport: {cc.Rect}},
The target view can then apply these value to itself, it's preferred not to modify directly its private variables
  - [`postApply`](#postapply) Manipulation after appyling the strategy
  - [`setContainerStrategy`](#setcontainerstrategy) Setup the container's scale strategy
  - [`setContentStrategy`](#setcontentstrategy) Setup the content's scale strategy



### Details


#### 属性（properties）


##### EXACT_FIT

> The entire application is visible in the specified area without trying to preserve the original aspect ratio.<br/>
Distortion can occur, and the application may appear stretched or compressed.

| meta | description |
|------|-------------|
| 类型 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> |
| 定义于 | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js:1420](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js#L1420) |



##### NO_BORDER

> The entire application fills the specified area, without distortion but possibly with some cropping,<br/>
while maintaining the original aspect ratio of the application.

| meta | description |
|------|-------------|
| 类型 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> |
| 定义于 | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js:1429](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js#L1429) |



##### SHOW_ALL

> The entire application is visible in the specified area without distortion while maintaining the original<br/>
aspect ratio of the application. Borders can appear on two sides of the application.

| meta | description |
|------|-------------|
| 类型 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> |
| 定义于 | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js:1438](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js#L1438) |



##### FIXED_HEIGHT

> The application takes the height of the design resolution size and modifies the width of the internal<br/>
canvas so that it fits the aspect ratio of the device<br/>
no distortion will occur however you must make sure your application works on different<br/>
aspect ratios

| meta | description |
|------|-------------|
| 类型 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> |
| 定义于 | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js:1447](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js#L1447) |



##### FIXED_WIDTH

> The application takes the width of the design resolution size and modifies the height of the internal<br/>
canvas so that it fits the aspect ratio of the device<br/>
no distortion will occur however you must make sure your application works on different<br/>
aspect ratios

| meta | description |
|------|-------------|
| 类型 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> |
| 定义于 | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js:1458](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js#L1458) |



##### UNKNOWN

> Unknow policy

| meta | description |
|------|-------------|
| 类型 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> |
| 定义于 | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js:1469](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js#L1469) |






<!-- Method Block -->
#### 方法


##### constructor



| meta | description |
|------|-------------|
| 定义于 | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js:1342](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js#L1342) |

###### 参数列表
- containerStg <a href="../classes/ContainerStrategy.html" class="crosslink">ContainerStrategy</a> The container strategy
- contentStg <a href="../classes/ContentStrategy.html" class="crosslink">ContentStrategy</a> The content strategy


##### preApply

Manipulation before applying the resolution policy

| meta | description |
|------|-------------|
| 定义于 | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js:1361](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js#L1361) |

###### 参数列表
- view <a href="../classes/View.html" class="crosslink">View</a> The target view


##### apply

Function to apply this resolution policy
The return value is {scale: [scaleX, scaleY], viewport: {cc.Rect}},
The target view can then apply these value to itself, it's preferred not to modify directly its private variables

| meta | description |
|------|-------------|
| 返回 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Object" class="crosslink external" target="_blank">Object</a> 
| 定义于 | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js:1371](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js#L1371) |

###### 参数列表
- view <a href="../classes/View.html" class="crosslink">View</a> The target view
- designedResolution <a href="../classes/Size.html" class="crosslink">Size</a> The user defined design resolution


##### postApply

Manipulation after appyling the strategy

| meta | description |
|------|-------------|
| 定义于 | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js:1385](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js#L1385) |

###### 参数列表
- view <a href="../classes/View.html" class="crosslink">View</a> The target view


##### setContainerStrategy

Setup the container's scale strategy

| meta | description |
|------|-------------|
| 定义于 | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js:1395](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js#L1395) |

###### 参数列表
- containerStg <a href="../classes/ContainerStrategy.html" class="crosslink">ContainerStrategy</a> 


##### setContentStrategy

Setup the content's scale strategy

| meta | description |
|------|-------------|
| 定义于 | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js:1405](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/platform/CCView.js#L1405) |

###### 参数列表
- contentStg <a href="../classes/ContentStrategy.html" class="crosslink">ContentStrategy</a> 



