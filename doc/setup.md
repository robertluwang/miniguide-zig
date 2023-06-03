test env is ubuntu vm on top of hyper-v 

## install zig 
$ sudo snap install zig --classic --beta

zig (beta) 0.10.1 from Jay Petacat (jayschwa) installed

$ which zig

/snap/bin/zig

## hello world 
$ mkdir -p ~/code/zig/helloworld

$ cat main.zig 
```
const std = @import("std");

pub fn main() void {
    std.debug.print("Hello, {s}!\n", .{"World"});
}
```

$ zig run main.zig

Hello, World!
