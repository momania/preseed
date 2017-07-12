### Preseeding Notes

## Make ISO
sudo mkisofs -R -J -v -T -no-emul-boot -boot-load-size 4 -boot-info-table -joliet-long -o ~/ubuntu/ubuntu-16.04.2-nvision.iso -b isolinux/isolinux.bin -c isolinux/boot.cat -V "nVision Ubuntu 16.04.2 Server" .
