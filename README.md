# Kali-Linux-ISH-SHELL
apk add gnupg
wget -O - https://http.kali.org/kali/keyrings/archive-keyring.asc | gpg --import
wget -O - https://http.kali.org/kali/pool/main/k/kali-archive-keyring/kali-archive-keyring-2020.2_all.deb | tar zxvf - ./usr/share/keyrings
cp ./usr/share/keyrings/kali-archive-keyring.gpg /usr/share/keyrings
echo "deb [signed-by=/usr/share/keyrings/kali-archive-keyring.gpg] https://http.kali.org/kali kali-rolling main non-free contrib" >> /etc/apk/repositories
