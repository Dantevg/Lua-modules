# How to use

I don't think you really should use any of this. There are lots of better built modules that perform the same tasks, and better.
This is just my attempt at making everything for myself (aka reinventing the wheel).  
However, if you still want to use my modules, go ahead:

```lua
-- For most modules (exclude .lua file extension)
local myModule = require "path/to/moduleName"

-- The 'utils' module puts its functions directly into the global env (exclude .lua file extension)
require "path/to/utils"

-- Rest of your code goes here, for example with the matrix module:
local m = myModule.new(3,2)

m:loop(function(val)
	return constrain( val, 0, 1 )
end)
```
