The GPG KEY Setup is here.


git config --global user.name "RanaUniverse"
git config --global user.email "RanaUniverse321@gmail.com"
gpg --list-secret-keys --keyid-format=long
gpg --full-generate-key

gpg --list-secret-keys --keyid-format=long


sec   rsa2016/ABC123XYZ789RANA 2024-10-26 [SC] [expires: 2024-11-10]
      987XYZ123ABCRANA123ABC78ABC123XYZ789RANA
uid                 [ultimate] RanaUniverse ("GPG key making for testing for github") <RanaUniverse321@gmail.com>
ssb   rsa2016/XYZ123ZYX987RANA 2024-10-26 [E] [expires: 2024-11-10]

gpg --armor --export ABC123XYZ789RANA
git config --global user.signingkey ABC123XYZ789RANA
git config --global commit.gpgsign true