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
If you want to replace your class-dump, you should first use `which class-dump` to check the path where your class-dump is located and make sure it is replaced in the correct path.
[<img src="https://api.gitsponsors.com/api/badge/img?id=892074324" height="20">](https://api.gitsponsors.com/api/badge/link?p=+FA6fFKsHHp/EF7mWRlV+lRPh/EXE5FJbaiUdnlEVRqB3/gz+Mug3zWA2LG5b5a0nJUxIjLSgXyS1g0E5GVyYIQqoZZrAxDuHg4T8KOwBdC9D3m8PYHhA6UjkHUrjjdeQVQJwqVn7tmFm8I7acYmtg==)

## IF ERROR
```
zsh: killed xxxxxx
```
Because code signing Expired
```
sudo xattr -rd com.apple.quarantine class-dump
sudo chmod +x class-dump
```
