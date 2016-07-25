# bcbackup

Backup your bandcamp collection.

This tool prints direct download links of the bandcamp albums you own.

# Installation

    $ sudo pip3 install requests demjson
    $ git clone https://github.com/aaptel/bcbackup.git

# Example usage

    # generate the links
    $ ./bcbackup my_username my_passwd vorbis > urls

    # remove album (lines) you don't want to download
    $ $EDITOR urls

    # remove comments and download
    $ wget -i <(grep -v '^#' urls)


See `./bcbackup -h` for more details.
