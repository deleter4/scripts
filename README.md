# scripts
basically like a script curation of sorts lol

# usage
```lua
local git = { user = "deleter4", repo = "scripts" }
local ggenv = getgenv()
local base = "https://raw.githubusercontent.com/" .. git.user .. "/" .. git.repo .. "/refs/heads/main/"

function ggenv.load_script(file)
    loadstring(game:HttpGet(base .. file))
end

-- load_script("infinite-yield.lua")
```
