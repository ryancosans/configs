# Configs

a simple repo to hold all the configs for things I use

# Generic

- install [docker](https://www.docker.com/products/docker-desktop)
- install [vscode](https://code.visualstudio.com/)

```bash
git config --global alias.co checkout
git config --global user.name "Your Name"
git config --global user.email you@example.com
```

kill the ports!
```bash
kill $(lsof -t -i :portno)
```

launch chrome in super sneaky mode

```bash
open -a Google\ Chrome --args --incognito --disable-web-security --user-data-dir --disable-features=CrossSiteDocumentBlockingIfIsolating,CrossSiteDocumentBlockingAlways
```

fuck with the power management settings using
```bash
pmset
```

---

## Sub modules

```bash
git submodule update --init --recursive
```
---

## Styles

 [![draculatheme](/dracula/dracula.gif)](https://draculatheme.com/)

 ---

# Java

## Sdkman

Simply open a new terminal and enter:

```bash
curl -s "https://get.sdkman.io" | bash
```

Follow the instructions on-screen to complete installation.
Next, open a new terminal or enter:

```bash
source "$HOME/.sdkman/bin/sdkman-init.sh"
```

install java
```bash
sdk list java
```

```bash
sdk install java [version]
```

## Raw
info stolen from [Solarian Programmer](https://solarianprogrammer.com/2018/09/28/installing-openjdk-macos/)

Start by getting [OpenJDK](http://jdk.java.net/11/), chose the macOS version. Extract the archive by double clicking on the file or, assuming it is in your Downloads folder, write this in your Terminal:

```bash
cd ~/Downloads
```
```bash
tar xf openjdk-11.0.2_osx-x64_bin.tar.gz
```

Next step, is to move the extracted folder to a place where macOS searches for Java JDK:

```bash
sudo mv jdk-11.0.2.jdk /Library/Java/JavaVirtualMachines/
```
Now, check if you’ve successfully installed the JDK with:

```bash
java -version
```