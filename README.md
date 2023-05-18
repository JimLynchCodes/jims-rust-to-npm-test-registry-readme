# jims-rust-to-npm-test-registry-readme
A test of using s different README with the rust-to-npm package for deplying rust cli tools to npm (and cargo)

---

Recreate this project with these steps:

## Step 1) Create a new repo
Create a new repo and clone it

## Step 2) Create a new rust binary project
This can easily be done with cargo:
```bash
cargo new jims-rust-to-npm-test-registry-readme
```

## Step 3) Change the hello message
Open the `main.rs` file and change the string returned to whatever you like...

## Step 4) Adjust Cargo.toml
Add these keys to Cargo.toml (with your desired values):
```
description = "A nice package description."
repository = "https://github.com/JimLynchCodes/jims-rust-to-npm-test-registry-readme"
readme = "README.registry.md"
keywords = ["rust-to-npm-cli", "deploy-rust", "npm", "rust", "cli-tool"]
categories = ["command-line-utilities"]
license = "MIT"
homepage = "https://github.com/JimLynchCodes/jims-rust-to-npm-test-registry-readme"
authors = ["Jim Lynch - jim.lynch@evaluates2.com"]
```

# Step 5) Account Logins

Login to your crates.io account in your terminal:
```sh
cargo login
```

Login to your npmjs.com account in your terminal:
```sh
npm adduser
```

## Step 6) Install rust-to-npm
```sh
cargo install rust-to-npm-cli
```

OR via npm (but not both)

```sh
npm i -g rust-to-npm-cli
```

## Step 7) Deploy With Other Name
```sh
rust-to-npm-cli deploy -b -n jims-registry-readme-cli
```

## Step 8) Re-Deploy
Change the version in Caargo.toml (according to semver) and then repeat step 6.

## Step 9) Install Your Package

```sh
npm i -g jims-registry-readme-cli
```

_or_

```sh
cargo install jims-registry-readme-cli
```

## Step 10) User Your Package

```sh
jims-registry-readme
```