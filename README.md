<p align = "center"> <img src="/pctf.png"/> </p>

___

### Static ain't always noise - 20 Points
#### Can you look at the data in this binary: `static`? This `BASH script` might help!

> Running the BASH script will generate `.ltdis.x86_64.txt` inside the current location. Looking into the BASH code was also useless for my case.
> I ran the `Format-Hex .\static` command on Powershell, to see the static in binary, I noticed some hints in there and after scrolling deeper into it, I found the flag.

> 00001020   70 69 63 6F 43 54 46 7B 64 31 35 61 35 6D 5F 74 \
> picoCTF{d15a5m_t \
> 00001030   33 34 73 33 72 5F 39 38 64 33 35 36 31 39 7D 00 \
> 34s3r_98d35619}. \
> 00001040   47 43 43 3A 20 28 55 62 75 6E 74 75 20 37 2E 35  GCC: \
> (Ubuntu 7.5 \
> 00001050   2E 30 2D 33 75 62 75 6E 74 75 31 7E 31 38 2E 30 \
> .0-3ubuntu1~18.0 \
> 00001060   34 29 20 37 2E 35 2E 30 00 00 00 00 00 00 00 00  4)

#### 🚩 picoCTF{d15a5m_t34s3r_98d35619}

## ©️ License:
Copyright © Kemal Demirgil. All rights reserved.
Licensed under the [MIT](https://github.com/kemaldemirgil/picoCTF/blob/main/LICENSE) license.
