# Entity options
```lua
exports.qtarget:AddTargetBone(bones, parameters)
```
##### Registers the defined options to display on all vehicles with the selected target bone.
###### Bones can be found in qtarget/data/bones.lua

```lua

exports.qtarget:AddTargetBone({'boot'},{
	options = {
		{
			event = "get:intrunk",
			icon = "fas fa-truck-loading",
			label = "Get in Trunk",
			num = 1
		},
		{
			event = "eventname",
			icon = "fas fa-box-circle-check",
			label = "action 2",
			num = 2
		},
	},
	distance = 2
})
```
##### Remove the target bone after usage.

```lua
exports.qtarget:RemoveTargetBone({'boot'}, {
    'Get in Trunk', 'action 2'
})
```
