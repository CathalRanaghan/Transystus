# Transystus

Safely migrate between Linux distribution flavours without a clean install.

> ⚠️ **Alpha Software** — This is early stage software. Use at your own risk.
> Before running **any** script, it is **strongly recommended** to:
> * Take a system backup using a utility of your own choice if testing on a physical machine
> * Take a snapshot to restore from if testing on a virtual machine (VM)
> * Avoid running scripts on a production or mission-critical system

---

## What Transystus Does

Transystus provides migration scripts that convert your existing Ubuntu installation
between flavours without requiring a clean install.

## What Transystus Does Not Do

- Guarantee perfect restoration of your pre-migration system state should you use a script to switch back to your original flavour
- Perform Ubuntu version upgrades — use `do-release-upgrade` for that
- Check your source system before migrating — There are currently no checks for migrating to a flavour you are already on, but this feature is planned
- Support distributions other than Ubuntu 26.04 LTS Desktop and Server at this time

---

## Supported Distributions

| Source | Target | Status |
|--------|--------|--------|
| Ubuntu 26.04 LTS Desktop | Ubuntu 26.04 LTS Server | ✅ Supported |
| Ubuntu 26.04 LTS Server | Ubuntu 26.04 LTS Desktop | ✅ Supported |

Bidirectional and non-pristine source system migrations are welcome for
community testing, but reliability and accuracy is not guaranteed.

A system is considered non-pristine if modifications to it are made that are not supported by the distribution maintainers, including previous migrations performed using the provided scripts.

---

## Requirements

- Ubuntu 26.04 LTS
- A user authorised to use `sudo` or `doas`
- A pristine or close to pristine source system is strongly recommended
- Running scripts as root is **not** recommended

---

## Usage

Migrate to Ubuntu Desktop:
    ./install-ubuntu-desktop

Migrate to Ubuntu Server:
    ./install-ubuntu-server
    
---

## Contributing

Community testing and contributions are welcome. Transystus is in early
stages and team members will be brought in organically as the project grows 
and contributors consistently show meaningful contributions.

---

## License

Transystus is licensed under the GNU General Public License v3.0 or later.
See [LICENSE](LICENSE) for details.

## Trademarks & Disclaimers

Transystus is an independent community project and is not affiliated with,
endorsed by, or associated with Canonical Ltd. or the Free Software Foundation (FSF).

Ubuntu is a registered trademark of Canonical Ltd. Linux is a registered
trademark of Linus Torvalds. GNU and related marks are trademarks of the
FSF. All trademarks are the property of their respective owners.
