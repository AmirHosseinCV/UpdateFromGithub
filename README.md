Keep your clients up to date by updating your projects from GitHub.

## Installation
You can easily add [UpdateFromGithub.py](https://github.com/AmirHosseinCV/UpdateFromGithub/blob/main/UpdateFromGithub.py) to your project and use it. But if you want to install it, you can use the following command:
```bash
pip install git+https://github.com/AmirHosseinCV/UpdateFromGithub.git
```
and for using without installation:
```bash
# using wget
wget https://raw.githubusercontent.com/AmirHosseinCV/UpdateFromGithub/main/UpdateFromGithub.py
# using curl
curl -o UpdateFromGithub.py https://raw.githubusercontent.com/AmirHosseinCV/UpdateFromGithub/main/UpdateFromGithub.py
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
