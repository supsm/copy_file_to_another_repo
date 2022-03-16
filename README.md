# copy_file_to_another_repo
Github Action to copy a file to another repository

## Examples/Variables
See [dmnemec/copy_file_to_another_repo_action](https://github.com/dmnemec/copy_file_to_another_repo_action/blob/main/README.md)  
### Additional Variables
fetch_depth: [optional] Number of commits to fetch (`--depth` argument in git). Defaults to 1.  

## Why
**TLDR:**  
- Alternative to [dmnemec/copy_file_to_another_repo_action](https://github.com/dmnemec/copy_file_to_another_repo_action) which works on all platforms  
- Same inputs as [dmnemec/copy_file_to_another_repo_action](https://github.com/dmnemec/copy_file_to_another_repo_action), simply replace `dmnemec/copy_file_to_another_repo_action@master` with `supsm/copy_file_to_another_repo@master` in workflows  

I created this as an alternative to [dmnemec/copy_file_to_another_repo_action](https://github.com/dmnemec/copy_file_to_another_repo_action) as it used a container action (Docker) and was therefore only usable on linux. My workflow needed to also copy files from Windows/Mac. There was nothing that worked at the time, so I created this action for my own convenience. Some of the commands are copied directly, and the inputs should also be the same (with some additions). For this reason, this action is also licensed under Apache-2.0.  
This action is a composite action instead of a docker action, therefore it is usable on non-linux platforms. However, since this was created for my own convenience, I may not be too quick to update things, and the action may break. If this does happen, please open an issue.  
