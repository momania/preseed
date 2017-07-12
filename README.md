### Preseeding Notes

#### Changes to original image

- Put customized seed file in `/preseed`
- Change timeout to `1` in `/isolinux/isolinux.cfg` (this skips the language select)
- Change `/isolinux/txt.cfg`, see sample in this repo

#### Make ISO

`sudo mkisofs -R -J -v -T -no-emul-boot -boot-load-size 4 -boot-info-table -joliet-long -o ~/ubuntu/ubuntu-16.04.2-custom.iso -b isolinux/isolinux.bin -c isolinux/boot.cat -V "Custom Ubuntu 16.04.2 Server" .`
