change regex for finding provision 

"provisionName"
'provisionName'
'provision-name'

include apostroph ' and -
local provision_name = line:match('.vm.provision[ \r\t]+[\"|\']([A-z]+[A-z0-9|-]*)[\"|\']')
