<h2 align="center">
  ALPHA - NOT READY FOR USE
  <br/>
  <a href="https://linux-dash.github.io">Linux Dash</a>
</h2>

<p align="center">
  <small>A simple & low-overhead web dashboard for linux systems</small>
</p>

<h4 align="center"><a href="https://linux-dash.github.io">linux-dash.github.io</a></h4>

<p align="center">
  <small>
    <a href="https://linux-dash.github.io/demo">Demo</a> &nbsp;|&nbsp;
    <a href="https://linux-dash.github.io">Features</a> &nbsp;|&nbsp;
    <a href="https://linux-dash.github.io/docs#installation">
      Installation
    </a>
  </small>
</p>


<p align="center">
  <a href="https://gitter.im/afaqurk/linux-dash">
    <img
      src="https://badges.gitter.im/gitterHQ/gitter.png"
      alt="linux-dash Gitter chat">
  </a>
</p>

<br/>

## Features
* **Small** ----- Under 400KB on disk _(with .git removed)!
* **Simple** --- A minimalist, beautiful dashboard
* **Easy** ------ Drop-in installation
* **Versatile** - _Choose your stack:_ Node.js, Go, C, Python, PHP, Binary

## Installation

### Step 1
```sh
## 1. clone the repo
git clone --depth 1 https://github.com/linux-dash/linux-dash.git

## 2. go to the cloned directory
cd linux-dash/app/server

```
OR, if you prefer to download manually:

```sh
## 1. Download the .zip
curl -LOk https://github.com/afaqurk/linux-dash/archive/master.zip && unzip master.zip

## 2. navigate to downloaded & unzipped dir
cd linux-dash-master/app/server

```

### Step 2

See instructions for stack you prefer to run linux-dash on:

* [Node.js](#nodejs) _(recommended)_
* [Go](#go)
* [Python](#python)
* [C](#c)
* [PHP](#php)

<br/>
#### Step 2: Node.js

```sh
## install dependencies
npm install --production

## start linux-dash (on port 80 by default; may require sudo)
node index.js

```

<br/>
#### Step 2: Go
```sh
## start the server (on port 80 by default; may require sudo)
go run index.go
```

To build a binary, run `go build && ./server -h`. See [@tehbilly](https://github.com/sergeifilippov)'s notes [here](https://github.com/afaqurk/linux-dash/pull/281) for binary usage options

<br/>
#### Step 2: Python

```sh
# Start the server (on port 80 by default; may require sudo).
python index.py
```

<br/>
#### Step 2: C

```sh
# extract the c server source files
tar -jxvf c_server.tar.bz2 -C ./

# compile the binary
cd c_server && make

# Start the server (on port 80 by default; may require sudo)
./index
```

<br/>
#### Step 2: PHP
(TODO: Update PHP instructions with snippets for nginx & apache configs)

1. Make sure you have the `exec`, `shell_exec`, and `escapeshellarg` functions enabled
2. Point your web server to `app/` directory under `linux-dash`
2. Restart your web server (Apache, nginx, etc.)
  - For PHP + Apache setup follow the [Digital Ocean tutorial](https://www.digitalocean.com/community/tutorials/how-to-install-linux-dash-on-ubuntu-14-04).
  - For help with nginx setup, see [this gist](https://gist.github.com/sergeifilippov/8909839) by [@sergeifilippov](https://github.com/sergeifilippov).

## Support

For general help, please use the [Gitter chat room](https://gitter.im/afaqurk/linux-dash).

## Security

**It is strongly recommended** that all linux-dash installations be protected via a security measure of your choice.


linux-dash does not provide any security or authentication features.
