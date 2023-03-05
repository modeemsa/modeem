## Modeem
Modeem web framework for nonprofit organization

## Installation
### Python
Modeem requires Python 3.8 or later to run. Use your package manager to download and install Python 3 on your machine if it is not already done

```sh
python3 --version
```
```sh
pip3 --version
```
### PostgreSQL
Modeem  uses PostgreSQL as database management system. Use your package manager to download and install PostgreSQL (supported version: 11.0 and later).
On Debian/Unbuntu, it can be achieved by executing the following:
```sh
sudo apt install postgresql postgresql-client
```
By default, the only user is postgres but Modeem forbids connecting as postgres, so you need to create a new PostgreSQL user:
```sh
 sudo -u postgres createuser -s modeem
```
### Modeem Code
Copy the Modeem code to your machine by executing the following:

```sh
 git clone git@github.com:modeemsa/modeem.git
```

### Dependencies
For libraries using native code, it is necessary to install development tools and native dependencies before the Python dependencies of Modeem. They are available in -dev or -devel packages for Python, PostgreSQL, libxml2, libxslt1, libevent, libsasl2 and libldap2.
On Debian/Unbuntu, the following command should install all the required libraries:
```sh
  sudo apt install python3-dev libxml2-dev libxslt1-dev libldap2-dev libsasl2-dev \
    libtiff5-dev libjpeg8-dev libopenjp2-7-dev zlib1g-dev libfreetype6-dev \
    liblcms2-dev libwebp-dev libharfbuzz-dev libfribidi-dev libxcb1-dev libpq-dev
```
Modeem  dependencies are listed in the [requirements.txt](requirements.txt)

```sh
 pip3 install -r requirements.txt
```
Installing nodeJS NPM and rtlcss for LTR support

```sh
sudo apt-get install nodejs npm -y
sudo npm install -g rtlcss
```
### Running Modeem
Once all dependencies are set up, Modeem can be launched by running [modeem-bin](modeem-bin), the command-line interface of the server.

```sh
 ./modeem-bin
```
## License

GNU/General Public License (see [license.txt](license.txt))

The Modeem code is licensed as GNU General Public License (v3) and the Documentation is licensed as Creative Commons (CC-BY-SA-3.0) and the copyright is owned by Modeem and Contributors.

By contributing to Modeem, you agree that your contributions will be licensed under its GNU General Public License (v3).

