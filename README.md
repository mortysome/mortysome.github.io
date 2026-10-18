# mortysome

```
morty@debian:~$ whoami
morty — cybersecurity, linux, programming. ctf, osint, homelab, hardware.
```

Source for my personal site: a portfolio that behaves like a Linux terminal. Scroll it like a normal page, or type commands and poke around.

**Live:** [mortysome.github.io](https://mortysome.github.io)

## What's in it

- **A working terminal** that opens with `neofetch` already run, with tab completion and command history
- **`nmap mortysome.fun`** runs a fake port scan where each open port leads to a part of the site
- **`docker ps`** lists what my CasaOS homelab is running
- **`man morty`** prints the manual page
- **Backtick (`` ` ``)** jumps to the terminal from anywhere on the page
- Projects laid out like `ls -la`, a toolkit, and links to my GitHub, blog and LinkedIn
- A few easter eggs. `help` won't list them all.

It's also:

- Responsive, tested at phone widths
- Free of trackers and cookies
- Respectful of reduced-motion settings
- Still readable without JavaScript, though the terminal needs it

## Built with

- HTML, CSS and vanilla JavaScript in a single `index.html`
- [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) and [IBM Plex Sans](https://fonts.google.com/specimen/IBM+Plex+Sans) from Google Fonts

There's no framework, no build step and no dependencies.

## Run it locally

```bash
git clone https://github.com/mortysome/mortysome.github.io.git
cd mortysome.github.io
python3 -m http.server 8000
```

Then open <http://localhost:8000>. Opening `index.html` directly in a browser works too.

## Editing

Everything lives in `index.html`:

- **Page sections**: edit the HTML under `<main>`
- **Terminal text**: the `PROFILE` and `FILES` objects in the script
- **New commands**: add an entry to `COMMANDS`
- **Colours and fonts**: the tokens in `:root` at the top of the `<style>` block

## Contributing

Found a bug, or have an idea for a command? Open an issue or a pull request.

## License

Free and open source. See [LICENSE](LICENSE).
