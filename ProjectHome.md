Read **register** state of a given process from within ruby

About reginfo [here](http://cipher.org.uk/2009/08/19/read-registers-with-ruby/)

**Example**
```
require 'reginfo'  
include  RegInfo  

pid = fork do  
system("tail -f txt")  
end  
  
puts getr("eip",pid) #here we get EIP  
```