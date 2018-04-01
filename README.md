# AriaNg-for-LEDE/OpenWrt

A LEDE/OpenWrt package of [AriaNg](https://github.com/mayswind/AriaNg).

## This repo WILL NOT update anymore(2018/04/01)

## Usage

### LEDE

Add `src-git custom https://github.com/akaxxi/AriaNg-for-LEDE.git` to `feed.conf.default`

Update and install the package:

```
./script/feeds update custom
./script/feeds install aria-ng
```

After the compilation is finished, you can find the `.ipk` file in the `bin/packages` directory. 

