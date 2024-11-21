# class-dump-bin
This is a bin raw for new Mach-O LoadCommand LC_REQ_DYLD 0x33, 0x34 `GREATER THAN` `iOS15`，
to solve this `fucking ERROR` when dump headers from Mach-O file，cause dyld chained fixups！
```
Unknown load command: 0x80000034 //LC_DYLD_CHAINED_FIXUPS (0x34 | LC_REQ_DYLD) /* used with linkedit_data_command */
Unknown load command: 0x80000033 //LC_DYLD_EXPORTS_TRIE (0x33 | LC_REQ_DYLD) /* used with linkedit_data_command, payload is trie */
Unknown load command: 0x00000032 //LC_BUILD_VERSION 0x32 /* build for platform min OS version */
Error: Cannot find offset for address 0x10000125032562 in dataOffsetForAddress:
```
## Usage
Same like [class-dump](https://github.com/nygard/class-dump)
```
./class-dump -H <Macho-O path> -o <output path>
```
