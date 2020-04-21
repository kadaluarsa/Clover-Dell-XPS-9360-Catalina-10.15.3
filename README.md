# OSX-Dell-XPS-9360-Catalina-10.15

Dell XPS 9360

Status : <br/>
- Clover support 10.15.3 (Clover need to be update to latest version for support 10.15.4)<br/>
- Opencore support 10.15.4 <br/>

How to migrate from Clover to Opencore in easy way : <br/>
1.Delete all folder inside EFI partition.<br/>
2.Copy and Paste my EFI folder in this repository into your EFI parition.<br/>
<image src='https://raw.githubusercontent.com/kadaluarsa/OSX-XPS-9360-Catalina/master/asset/mypartition.png'/>
<br/>
3.Make sure only EFI folder inside EFI parition.<br/>
3.Reboot.<br/>

note : clear Clover NVRAM before migrate to Opencore.<br/>

Intel i7-7560U<br/>
16GB RAM LPDDR3<br/>
Sharp SHP144 LQ133Z1 QHD+ (3200x1800) Touchscreen display<br/>
Samsung SM961 SSD<br/>
Wifi replace with BCM943602CS<br/>
Samsung SM961 NVMe 512 sector better replace with NVMe 4k sector<br/>
Touchscreen (though it works out of the box if enabled)<br/><br/>
Optional : <br/>
Undervolt with voltageshift : <b>sudo ./voltageshift buildlaunchd -110 -110 -110 0 0 0 1 15 31 20</b><br/>
- reduce CPU,CPU cache,GPU to -110v (make more stable and reduce coilwhine when play 4K video)<br/> 
- enable turbo mode 1<br/>
- set TDP to 15 and turbo TDP to 31(fix TDP based on intel cpu information because default value is 17 and 33)<br/>
- repeat autojob every 20 minute<br/>
Download voltageshift here : https://drive.google.com/file/d/1v6woypx2APiejCVwaF9zwQhBHyICAHPY/view?usp=sharing<br/>
