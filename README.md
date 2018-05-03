# FirstGem
Its first gem that I created to be happy.


## Get started
Make clone of project or simply specify path in gemfile
 ```
 git clone https://github.com/dashingshakeel/FirstGem.git
```
## Installing
use this in gemfile
```
gem "dashing_gem", path: "https://github.com/dashingshakeel/FirstGem.git"
```
## How to create your own :+1:

First of all dont make it complicated its first time 

- Create .gemspec file with name of gem directory name and specifications about gem
In dashing_spec.gemspec file

```
Gem::Specification.new do |s|
  s.name = %q{dashing_gem}
  s.version = "0.0.0"
  s.date = %q{2018-05-03}
  s.platform      = Gem::Platform::RUBY
  s.authors       = ["Shakeel Rauf"]
  s.email         = ["shkeelrauf@gmail.com"]
  s.summary = %q{dashing_gem is the best}
  s.files = [
    "lib/dashing_gem.rb"
  ]
  s.require_paths = ["lib"]
end

```
- Create lib directory and file in lib directory with same name of gem and gemspec file.. **Simple CODE in that file **
```
module DashingGem
  class WhoIs
    def  self.dashing?
     puts  "Shakeel IS dashing"
    end
  end
end

```

- At last to build gem run following command in Command Shell with name of your gem
```
gem build dashing_gem.gemspec
```
