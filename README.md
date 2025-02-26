# setting up dev environment on macOS

## terminal config
- install omz:
    ```
    sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
    ```
    (check https://ohmyz.sh/#install if needed)
    - if prompted with "No developer tools were found, requesting install," install dev tools (i.e., git) -- should be prompted automatically
- terminal preferences: change startup profile to 'Homebrew;' change Homebrew settings to font size (18) and window columns/rows (100/24)
- install [powerlevel10k](https://github.com/romkatv/powerlevel10k) (follow all relevant instructions on p10k's readme)
- change default git text editor to nano: `git config --global core.editor "nano"`
- set git commit author info: `git config --global user.email INSERT EMAIL ADDRESS HERE`

## vs code config
- install vs code
- open command palette and search "shell command."  run "install 'code' command in PATH"
        - lets us use `code .` in terminal

## node config

## connect to github

- generate a new SSH key in the terminal: `ssh-keygen -t ed25519 -C "INSERT EMAIL ADDRESS HERE"`
- accept default file directory
- submit preferred passphrase
- copy public key: `pbcopy < ~/.ssh/id_ed25519.pub`
- add new SSH key on github