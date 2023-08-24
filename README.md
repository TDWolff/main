# Simple Guide: Setting Up GitHub Pages and Jekyll Blog

## GitHub Pages & Jekyll

1. GitHub Pages hosts websites from GitHub repos.
2. Jekyll makes content static sites.
3. Changes trigger auto build & publish.

## Local Testing (Development Cycle)

1. **Test Locally**: Try changes on your PC.
2. **Preview**: See changes before committing.

## Deployment (Deployment Cycle)

1. **Complete Dev Cycle**.
2. **Sync**: Use VSCode to sync changes.
3. **GitHub Update**: Triggers Jekyll build.
4. **Errors Possible**: Review if needed.

## Setup for WSL/Ubuntu

```bash
# Install Ruby, Python, Jupyter
sudo apt update
sudo apt install -y ruby-full build-essential zlib1g-dev python3 python3-pip python-is-python3 jupyter-notebook

# Install Ruby Gems & Jekyll
export GEM_HOME="$HOME/gems"
export PATH="$HOME/gems/bin:$PATH"
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
gem install jekyll bundler
