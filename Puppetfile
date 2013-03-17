# This file manages Puppet module dependencies.
#
# It works a lot like Bundler. We provide some core modules by
# default. This ensures at least the ability to construct a basic
# environment.

def github(name, version, options = nil)
  options ||= {}
  options[:repo] ||= "boxen/puppet-#{name}"
  mod name, version, :github_tarball => options[:repo]
end

# Includes many of our custom types and providers, as well as global
# config. Required.

github "boxen", "1.2.0"

# Core modules for a basic development environment. You can replace
# some/most of these if you want, but it's not recommended.

github "dnsmasq",  "1.0.0"
github "gcc",      "1.0.0"
github "git",      "1.1.0"
github "homebrew", "1.1.2"
github "hub",      "1.0.0"
github "inifile",  "1.0.0"
github "nginx",    "1.1.0"
github "nodejs",   "1.0.0"
github "nvm",      "1.0.0"
github "ruby",     "3.3.1"
github "stdlib",   "3.2.0", :repo => "puppetlabs/puppetlabs-stdlib"
github "sudo",     "1.0.0"

# Optional/custom modules. There are tons available at
# https://github.com/boxen.
github "java",     "1.0.6"
github "caffeine", "1.0.0"
github "wget",     "1.0.0"
github "fluid",    "1.0.0"
github "chrome",   "1.1.0"
github "skype",    "1.0.1"
github "flux",     "0.0.1"
github "dropbox",  "1.1.0"
github "sourcetree", "1.0.0", :repo => "oneboxmedia/boxen-sourcetree"
