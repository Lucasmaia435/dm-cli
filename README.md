# Deno-cli

## Commands
```bash
..>dm --help
Usage: index [options] [command]

Options:
  -V, --version   output the version number
  -h, --help      display help for command

Commands:
  init            Initiate a deno project
  run             Run your deno project
  help [command]  display help for command
  ```

## `init`
Create a workspace with two files: index.ts and config.json.

### Config.json contains the fields "main" and "permissions":
```json
{
    "main":"index.ts",
    "permissions":[
        "--allow-net"
    ]
}
```
In this file you should add all the permissions that you need.

### Index.ts
```typescript
console.log("Hello world!");
```