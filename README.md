# reginfo
Read register state of a given process from within ruby

https://github.com/cphr/reginfo/releases/download/0.1/reginfo-src.tar.gz
https://github.com/cphr/reginfo/releases/download/0.1/reginfo.so.gz

Example 

```ruby 
require 'reginfo' 
include RegInfo

pid = fork do 
system("tail -f txt") 
end

puts getr("eip",pid) #here we get EIP 
```
