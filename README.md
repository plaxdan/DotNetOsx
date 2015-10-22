# DotNetOsx

The simplest possible .Net project that will run on OSX.

## Install dnvm

Install .Net Version Manager. This will add a line to your [`zshrc`](https://github.com/plaxdan/prezto/commit/8b6b16171453232aea5b0a876daf1b668ccfd5f2).

```
curl -sSL https://raw.githubusercontent.com/aspnet/Home/dev/dnvminstall.sh | DNX_BRANCH=dev sh && source ~/.dnx/dnvm/dnvm.sh
```

## Install the Core CLR

Use `dnvm` to install either mono or the Core CLR.

```
dnvm upgrade -r coreclr
```

## Install Dependencies

This will download dependencies defined in `project.json`.

```
dnu restore
```
