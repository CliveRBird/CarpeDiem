# CarpeDiem
Scaffold code snippits.

export GPG_TTY=$(tty)

tar czvpf - file1.txt file2.pdf file3.jpg | gpg --symmetric --cipher-algo aes256 -o myarchive.tar.gz.gpg

gpg -d myarchive.tar.gz.gpg | tar xzvf -
