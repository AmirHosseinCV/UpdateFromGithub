Update your projects automatically from GitHub.

## Installation
```commandline
pip install git+https://github.com/AmirHosseinCV/UpdateFromGithub.git
```

## Usage

```python
from UpdateFromGithub import Repository
repo = Repository(repo_owner="AmirHosseinCV",
                  repo_name="UpdateFromGithub",
                  branch="main",
                  local_dir=".")
if repo.check_for_updates():
    repo.auto_update()
```
That's it!