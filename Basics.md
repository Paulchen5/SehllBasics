# Basic Shell Commands and Usages

### Redirecting output to a file
<!-- See https://stackoverflow.com/questions/6762348/what-do-and-do-in-tcsh#answer-6762399 -->
If `noclobber` is set:https://github.com/Paulchen5/SehllBasics/tree/main
- `cmd > file` will write `stdout` to file if file does not exist
- `cmd > file` will fail if file exists
- `cmd >> file` will append `stdout` to file if file exists
- `cmd >> file` will fail if file does not exist
- `cmd >! file` will write `stdout` to file, overwriting any existing file
- `cmd >>! file` will append `stdout` to file, creating the file if it does not already exist

If `noclobber` is not set then the ! has no effect:
- `cmd > file` will write `stdout` to file, overwriting any existing file
- `cmd >> file` will append `stdout` to file
- `cmd >! file` will write `stdout` to file, overwriting any existing file
- `cmd >>! file` will append `stdout` to file
