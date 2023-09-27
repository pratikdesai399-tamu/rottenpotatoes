# Rotten Potatoes

A simple app called RottenPotatoes (inspired by the real web site RottenTomatoes) for cataloging movies. RottenPotatoes lets users interactively (via a Web browser) create database entries for new movies, view or modify the content of movie records (movie title, rating, description, and so on), and delete movie records.

#Installation and Setup guide

1. Install rbenv
```
•	cd ~
•	curl -fsSL https://github.com/rbenv/rbenv-installer/raw/HEAD/bin/rbenv-installer | bash
```

2. Verify ~/.zshrc file contains the path variables, if not add them:
   
```   
export PATH=$HOME/.rbenv/bin:$PATH
eval export PATH="/Users/vinodheniramasrinivasan/.rbenv/shims:${PATH}"
export RBENV_SHELL=zsh
source '/Users/vinodheniramasrinivasan/.rbenv/completions/rbenv.zsh'
command rbenv rehash 2>/dev/null
rbenv() {
  local command
  command="${1:-}"
  if [ "$#" -gt 0 ]; then
    shift
  fi

  case "$command" in
  rehash|shell)
    eval "$(rbenv "sh-$command" "$@")";;
  *)
    command rbenv "$command" "$@";;
  esac
}
```
3. Reload zshrc :
```
source ~/.zshrc
```
   
4. Install Ruby :
```
rbenv install 3.2.2
```

5. Go to a ruby project folder

```
Set ruby 3.2.2 as the local default version: rbenv local 3.2.2
Set 3.2.2 as the global version : rbenv global 3.2.2
gem install bundler
```

6. Install the dependenices :
```
bundle install
```

7. Verify Ruby version :
```
ruby -v
```

8. Install Rails :
    
•	To install Rails, use the gem install command:
```
gem install rails
```

9. Create database :
```
rails db:create
```

•	Once completed, Verify by running:
```
rails -v
```

•	Run this command satrt the server locallay
```
rails server
```


