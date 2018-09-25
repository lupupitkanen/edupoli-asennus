# Edupoli harjoituksen asennusohjeita

## Asenna Virtualbox

https://www.virtualbox.org/wiki/Downloads

Mahdollisesti voidaan käyttää myös VMware Workstationia.

## Vagrant

https://www.vagrantup.com/downloads.html

Asenna tuplaklikkaamalla msi-tiedostoa ja anna pyydettäessä admin-tason tunnukset.

## Asenna Vagrant box Ubuntu desktop virtuaalikone

https://app.vagrantup.com/peru/boxes/ubuntu-18.04-desktop-amd64

1. Avaa komentokehto (`cmd`)
2. Komentokehotteessa aja:
```
mkdir ubuntu-18.04-desktop-amd64
cd ubuntu-18.04-desktop-amd64
vagrant init peru/ubuntu-18.04-desktop-amd64
vagrant up
```

## Kirjaudu Ubuntu virtuaalikoneeseen

Oletuksena tunnus ja salasana molemmat `vagrant`.

Tarvittaessa asenna suomen kieli ja vaihda näppäimistö suomalaiseksi.

## Luo SSH-avain

1. Avaa Terminal
2. Aja komento `ssh-keygen`
3. Voit jättää harjoituksessa passphrasen tyhjäksi

## Google Cloud SDK

Asenna Ubuntuun Google Cloud SDK:

https://cloud.google.com/sdk/docs/quickstart-debian-ubuntu

Testaa terminalissa kirjautumista:

```
gcloud auth application-default login
```

## Asenna Terraform

Asenna Ubuntuun Terraform:

https://www.terraform.io/intro/getting-started/install.html

```
wget https://releases.hashicorp.com/terraform/0.11.8/terraform_0.11.8_linux_amd64.zip
unzip terraform_0.11.8_linux_amd64.zip
sudo mv terraform /usr/local/bin/
terraform
```
