<div align="center">
    <h3>manual-install-guide<h3>
    <p>A collection for manual installations guide</p>
</div>

## Why? <!-- omit in toc -->
I'm too lazy to search the web for tool/lib/language manual installation how-tos (especially tools I had installed before).

## TOC <!-- omit in toc -->
- [deno](#deno)

## How-tos <!-- omit in toc -->

### deno

According to [denoland/deno_install](https://github.com/denoland/deno_install), we should follow these steps:

1. download and unzip deno release 
2. mkdir `$HOME/.deno` and `$HOME/.deno/bin`
3. copy executable file `deno` to  `$HOME/.deno/bin`
4. add environment variable `export $DENO_INSTALL=` and update `PATH` with `export $DENO_INSTALL/bin:$PATH`to shell configuration file like `.bashrc`, `.zshrc` etc 

Actually you could use `export DENO_INSTALL_ROOT="$HOME/.deno/bin"` instead of `$DENO_INSTALL`  so that you only need to update `PATH` with `export $DENO_INSTALL_ROOT:$PATH`

```md
ENVIRONMENT VARIABLES:
    DENO_DIR             Set the cache directory
    DENO_INSTALL_ROOT    Set deno install's output directory
                         (defaults to $HOME/.deno/bin)
    DENO_CERT            Load certificate authority from PEM encoded file
    NO_COLOR             Set to disable color
    HTTP_PROXY           Proxy address for HTTP requests
                         (module downloads, fetch)
    HTTPS_PROXY          Proxy address for HTTPS requests
                         (module downloads, fetch)
```