To download all repos from a git account

```
sudo gem install json
curl -s https://api.github.com/users/{ACC_USERAME}/repos?per_page=100 | ruby -rjson -e 'JSON.load(STDIN.read).each {|repo| %x[git clone #{repo["clone_url"]} ]}'
```
