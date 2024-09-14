SailfishOS HADK Scratchpad for lenovo_karatep
- based on lineage/hybris-18.1

Notes:
Add LOS devicesettings: https://github.com/tanvirr007/CustomROM_build_guide_aosp

Resources:
- (ofono conflict) https://sailfishos.wiki/books/hadk/page/hadk-hot https://irclogs.sailfishos.org/logs/%23sailfishos-porters/%23sailfishos-porters.2023-02-03.log.html
- (setup selinux permissive) https://piggz.co.uk/sailfishos-porters-archive/index.php?log=2024-08-20.txt#line64

Commands:
- (Update Platform SDK, Tooling, and Target): "sdk-foreach-su -ly ssu re some_version" then "sdk-foreach-su -ly zypper ref" and finally "sdk-foreach-su -ly zypper dup"

Patch apex:
- If apexd-bootstrap fails because of not updatable/flattened apexes here is experimental fix: https://paste.debian.net/hidden/a2302262/ (Thanks @elros34)
