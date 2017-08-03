## `PhysicsCollider` Class



Module: [cc](../modules/cc.md)
Parent Module: [cc](../modules/cc.md)






### Index

##### Properties

  - [`density`](#density) `Number` The density.
  - [`sensor`](#sensor) `Boolean` A sensor collider collects contact information but never generates a collision response
  - [`friction`](#friction) `Number` The friction coefficient, usually in the range [0,1].
  - [`restitution`](#restitution) `Number` The restitution (elasticity) usually in the range [0,1].
  - [`body`](#body) `RigidBody` Physics collider will find the rigidbody component on the node and set to this property.



##### Methods

  - [`apply`](#apply) Apply current changes to collider, this will regenerate inner box2d fixtures.
  - [`getAABB`](#getaabb) Get the world aabb of the collider



### Details


#### Properties


##### density

> The density.

| meta | description |
|------|-------------|
| Type | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> |
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/physics/collider/CCPhysicsCollider.js:52](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/physics/collider/CCPhysicsCollider.js#L52) |



##### sensor

> A sensor collider collects contact information but never generates a collision response

| meta | description |
|------|-------------|
| Type | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Boolean" class="crosslink external" target="_blank">Boolean</a> |
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/physics/collider/CCPhysicsCollider.js:70](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/physics/collider/CCPhysicsCollider.js#L70) |



##### friction

> The friction coefficient, usually in the range [0,1].

| meta | description |
|------|-------------|
| Type | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> |
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/physics/collider/CCPhysicsCollider.js:88](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/physics/collider/CCPhysicsCollider.js#L88) |



##### restitution

> The restitution (elasticity) usually in the range [0,1].

| meta | description |
|------|-------------|
| Type | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> |
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/physics/collider/CCPhysicsCollider.js:106](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/physics/collider/CCPhysicsCollider.js#L106) |



##### body

> Physics collider will find the rigidbody component on the node and set to this property.

| meta | description |
|------|-------------|
| Type | <a href="../classes/RigidBody.html" class="crosslink">RigidBody</a> |
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/physics/collider/CCPhysicsCollider.js:124](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/physics/collider/CCPhysicsCollider.js#L124) |






<!-- Method Block -->
#### Methods


##### apply

Apply current changes to collider, this will regenerate inner box2d fixtures.

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/physics/collider/CCPhysicsCollider.js:250](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/physics/collider/CCPhysicsCollider.js#L250) |



##### getAABB

Get the world aabb of the collider

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/physics/collider/CCPhysicsCollider.js:262](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/physics/collider/CCPhysicsCollider.js#L262) |



