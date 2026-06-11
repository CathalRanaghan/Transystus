### Current Roadmap

# Short Term
- [ ] Add source system checks
- [ ] Fix sorting of packages marked automatically and manually installed so they're alphabetical
- [ ] Update `/usr/lib/os-release` as part of the migration process
- [ ] Resolve permissions on copied files and directories within `/etc`
- [ ] Update instance locking method
- [ ] Use `-` instead of spaces for word separation in directories such as `Ubuntu Server Assets` or `Ubuntu Desktop Assets`
- [ ] Use all lowercase characters for file and directory names

# Medium Term
- [ ] Merge `install-ubuntu-desktop` and `install-ubuntu-server` into one script named `Transystus`
- [ ] Add user interaction elements that emulate install options for a clean Ubuntu system install (e.g. OpenSSH Server for Ubuntu Server, Default/Extended Selection for Ubuntu Desktop, etc.)
- [ ] Add support for other Ubuntu Flavours (Kubuntu, Xubuntu, Lubuntu, etc.)

# Long Term
- [ ] Move logic not directly tied to migration to Rust
