# WIP: Moss Package Recipe for the Zig Programming Language

## !!! Note: This is a work in progress as I explore how moss packaging works in AerynOS. !!!

## How to build
Assuming a local repo has been setup (https://aerynos.dev/packaging/workflow/basic-workflow/)

```shell
# Clone the git repo
git clone https://github.com/ChrisArmstrongUK/mosspkg-ziglang.git

# Change into the repo directory
cd mosspkg-ziglang

# Build the package and move into the local moss repo index
just build
just mv-local

# Sync moss repos and install
moss sync -u
moss install ziglang
```