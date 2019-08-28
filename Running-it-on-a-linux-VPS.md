1. Check [Setting up your own version](https://github.com/Ankrad/Discord-Bot-List/wiki/Setting-up-your-own-version)
2. Install nodejs, npm, git and nano:
```console
sudo apt update
sudo apt install nodejs npm git nano
```
3. Clone the repository:
```console
git clone https://github.com/Ankrad/Discord-Bot-List
```
4. Edit the environment variables in nano:
```console
cd Discord-Bot-List
nano .env
```
5. Save and exit:
`ctrl+x`
`y`
`enter`
6. Install the required dependencies:
```console
npm install
```
7. Run it:
```console
npm start
```