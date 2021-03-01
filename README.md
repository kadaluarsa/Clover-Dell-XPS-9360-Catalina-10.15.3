# OSX-Dell-XPS-9360-BigSur-LTS

Dell XPS 9360

Status : <br/>
- Opencore  <br/><br/>
*Mandatory<br/>
1.set pre-alloc "setup_var 0x785 to 0x04" it will set pre-alloc to (128MB) match with BIOS<br/>
2.if you want go above 128MB you have to set framebuffer-stolenmem=00000006. <br/>
3.link <a href="https://www.elitemacx86.com/threads/guide-how-to-unlock-dvmt-pre-allocated-on-laptops.313/">Guide to set DVMT</a><br/>
4.link <a href="https://github.com/zearp/optihack/blob/master/text/CFGLock_DVMT.md">DVMT pre-alloc sizes for iGPU(Max 1GB pre-alloc)</a><br/>
<br/>

How to migrate from Clover to Opencore in easy way : <br/>
1.Delete all folder inside EFI partition.<br/>
2.Copy and Paste (EFI_OC or EFI_CLOVER) into your EFI parition. *dont forget, rename it to EFI<br/>
3.Make sure only EFI folder inside EFI parition.<br/>
3.Reboot.<br/>

note : <br/>
- Clear Clover NVRAM before migrate to Opencore.<br/>
- Opencore give more stable system.<br/>

Intel i7-7560U<br/>
16GB RAM LPDDR3<br/>
Sharp SHP144 LQ133Z1 QHD+ (3200x1800) Touchscreen display<br/>
Samsung SM961 SSD<br/>
Wifi replace with BCM943602CS<br/>
Samsung SM961 NVMe 512 sector better replace with NVMe 4k sector<br/>
Touchscreen (though it works out of the box if enabled)<br/><br/>
