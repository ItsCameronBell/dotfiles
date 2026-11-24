# dotfiles

Personal config files, managed with [GNU Stow](https://www.gnu.org/software/stow/).

Each top-level folder is a stow package. Its contents mirror the paths under
`~`, and stow links them there as symlinks.

## Usage

Requires `stow` (`brew install stow`).

```sh
git clone <repo-url>
stow git            # link a package
stow -D git         # remove its links
stow -R git         # relink after adding or removing files
stow -n -v git      # dry run, shows what would happen
```
