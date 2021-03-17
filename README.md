# Provsioning

## Setup provsioning

Install ansible

```sh
$ ssh pi@raspberrypi.local "
    sudo apt-get update &&
    sudo apt-get install -y ansible
"
```

## Run provisioning

Run provisioning script

```sh
ssh pi@raspberrypi.local "
curl -sL https://github.com/tomorrowkey/raspberrypi/archive/master.tar.gz -o raspberrypi-master.tar.gz &&
tar -zxf raspberrypi-master.tar.gz &&
cd raspberrypi-master &&
ansible-playbook site.yml
"
```
