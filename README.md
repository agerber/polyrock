
# PolyRock - asteroids code translations
This repo contains the asteroids reference project translated into the following languages: 

[Completed]: Java, Kotlin, Python, GoLang, and Typescript
[Under development]: C++, Rust 

## add the submodules

```bash
  
  repos=(
    "asteroids_java"
    "asteroids_kotlin" 
    "asteroids_python" 
    "asteroids_typescript" 
    "asteroids_go" 
    # "asteroids_cpp" 
    # "asteroids_rust" 

  )

  base_url="git@github.com:agerber"

  for repo in "${repos[@]}"; do
    git submodule add --force "$base_url/$repo.git" "$repo"
  done

```


## if you need to reset them

```bash
  git submodule foreach --recursive git reset --hard
  git submodule update --init --force --recursive
```
