# class-dump-bin
This is a bin raw for new Mach-O LoadCommand LC_REQ_DYLD 0x33, 0x34 `GREATER THAN` `iOS15`，
to solve this `fucking ERROR` when dump headers from Mach-O file，cause dyld chained fixups！
```
Unknown load command: 0x80000034
Unknown load command: 0x80000033
Unknown load command: 0x00000032 
Error: Cannot find offset for address 0x10000125032562 in dataOffsetForAddress:
```
## Usage
Same like [class-dump](https://github.com/nygard/class-dump)
```
./class-dump -H <Macho-O path> -o <output path>
```
