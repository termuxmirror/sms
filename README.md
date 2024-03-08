# sms

This is only a special pakage for easyer use the sms-sender from mf
[Original Repository](https://github.com/mfr-fr/sms-sender)

This version is only for Linux/Termux

## Instruction

1. Download all things for sms-sender

Termux

```bash
pkg update && pkg upgrade
pkg install git
pkg install python3
git clone https://termuxmirror/sms
cd sms
mv sms-0.1.tar.gz $HOME
cd $HOME
mkdir sms-sender
mv sms-0.1.tar.gz sms-sender/
rm -r -f sms
cd sms-sender
pip install sms-0.1.tar.gz
nano main.py
```

Ubuntu Debian

```bash
sudo -i
```

```bash
apt update && apt upgrade
apt-get install git
apt-get install python3
git clone https://termuxmirror/sms
cd sms
mv sms-0.1.tar.gz $HOME
cd $HOME
mkdir sms-sender
mv sms-0.1.tar.gz sms-sender/
rm -r -f sms
cd sms-sender
pip3 install sms-0.1.tar.gz
nano main.py
```

2. Write main.py

```python
# main.py

from sms.sms_sender import menu

def main():
    menu()

if __name__ == "__main__":
    main()
```

3. Run 

Termux

```bash
python main.py
```

Ubuntu/Debian

```bash
python3 main.py
```