 
# AVAILABLE FUNCTIONS
 
preference.save

preference.getValue

preference.getAllValues

preference.print

preference.printAll
 
 
 
## USAGE AND EXAMPLES
 
preference = require "preference"
 
preference.save{a=1}
value = preference.getValue("a")
 
preference.save{b="1"}
value = preference.getValue("b")
 
preference.save{c=true}
value = preference.getValue("c")
 
preference.save{d = {1,"2",true}}
value = preference.getValue("d")




This library is specifically for lua as used in Corona SDK.
For general using in Lua,
replace 
	local path = system.pathForFile( fileName, system.DocumentsDirectory )
by 
	local path = fileName
in 2 places in preference.lua file