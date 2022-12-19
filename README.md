<p align="center">Windows Top 70 CMD Command</p>

## `ipconfig`

Ipconfig, DOS işletim sisteminde bilgisayarın ağ bağlantı özelliklerini gösteren komuttur.
```ipconfig```

## `ipconfig /all`

şeklinde kullanıldığında ağ bağlantısı özellikleri daha ayrıntılı görülebilir. /all parametresiyle birlikte kullanıldığında bilgisayarın MAC adresi de ekrana basılır.
```
ipconfig /all
```

## `ipconfig /release`

ipconfig /release dhcp'den dagıtılan ip adresini geri bırakır.
```
ipconfig /release
```

## `ipconfig /renew`

ipconfig /renew dhcp'den dagıtılan yeni ip adresi almaya yarar.
```
ipconfig /renew
```

## `ipconfig /displaydns`

Bu seçenekler, Windows'un sahip olduğu yerel bir DNS önbelleğine erişir. /Displaydns komutu önbelleğin içeriğini ekrana yazdırmak için kullanılırken, /flushdns ise seçeneğin (önbelleğini) içeriğini siler.
```
ipconfig /displaydns
```

## `clip`

Clip komutu , komut satırı araçlarının çıktısını Windows panosuna yönlendirir. Bu metin çıktısı daha sonra diğer programlara yapıştırılabilir.
```
ipconfig /all | clip
```

## `ipconfig /flushdns`

ipconfig /flushdns dns bellegini temizler.
```
ipconfig /flushdns
```

## `nslookup`

NSlookup komutu, bir sayfanın TCP/IP numarasını bulunmasına yardımcı olur.
```
nslookup
```

## `cls`

CMD ekranını temizlemeye yarayan komuttur.
```
cls
```

## `getmac /v`

Mac adreslerini getirmeye yaran komut.
```
getmac /v
```

## `powercfg /energy`

Bilgisayarınızın davranışını altmış saniye boyunca gözlemleyecek ve ardından mevcut sistem durumunuzun ne kadar güç açısından verimli olduğu hakkında bilgiler içeren bir HTML raporu oluşturacaktır.
```
powercfg /energy
```

## `powercfg /batteryreport`

Mevcut pilinizin gerçek kapasitesi ve kapasitesi ile pil ömrünün zaman içinde nasıl azaldığı hakkında bilgiler dahildir.
```
powercfg /batteryreport
```

## `assoc`

Tüm dosya uzantılarının ve bunların hangi programla açıldığının listeler.
```
assoc .log=txtfile
```

## `chkdsk /f`

Diskteki hataları düzeltir. Disk kilitlenmelidir. CHKDSK sürücüyü kilitleyemezse, bilgisayarı bir sonraki yeniden başlatışınızda sürücüyü kontrol etmek isteyip istemediğinizi soran bir mesaj görüntülenir.
```
chkdsk /f
```

## `chkdsk /r`

Bozuk sektörleri bulur ve okunabilir bilgileri kurtarır. Disk kilitlenmelidir. Fiziksel disk hatalarının ek analiziyle birlikte / f işlevini içerir.
```
chkdsk /r
```

## `chkdsk /x`

Gerekirse önce birimi kaldırmaya zorlar. Sürücünün tüm açık tutamaçları geçersiz kılınmıştır. Ayrıca / f işlevini de içerir.
```
chkdsk /x
```

## `chkdsk /b`

Yalnızca NTFS içindir. Birimdeki bozuk kümeler listesini temizler ve tüm ayrılmış ve boş kümeleri hatalar için yeniden tarar.  / r işlevini içerir. Bir birimi yeni bir sabit disk sürücüsüne imajladıktan sonra bu parametreyi kullanın.
```
chkdsk /b
```

## `chkdsk /v`

Disk kontrol edilirken her dizindeki her dosyanın adını görüntüler.
```
chkdsk /v
```

## `chkdsk /scan`

yalnızca NTFS içindir. Birimde çevrimiçi bir tarama çalıştırır.
```
chkdsk /scan
```

## `chkdsk /i`

Yalnızca NTFS içindir. CHKDSK'yi çalıştırmak için gereken süreyi azaltan dizin girişlerini daha yüzeysel bir şekilde kontrol eder.
```
chkdsk /i
```

## `chkdsk /c`

Yalnızca NTFS içindir. Klasör yapısı içindeki döngüleri kontrol etmez, bu da CHKDSK'yi çalıştırmak için gereken süreyi azaltır.
```
chkdsk /c
```

## `sfc /scannnow`  (System File Checker)

Komutu korunan tüm sistem dosyalarını tarar ve bozuk dosyaları %WinDir%\System32\dllcache dizinindeki bir sıkıştırılmış klasörde bulunan önbelleğe alınmış kopyasıyla değiştirir. %WinDir% yer tutucu, Windows işletim sistemi klasörünü gösterir. Örneğin, C:\Windows.
```
sfc /scannnow
```

## `DISM`

Deployment Image Servicing and Management (DISM) Aracı, Windows görüntünüzü onarmak veya Windows kurulum ortamınızı değiştirmek için Windows'da kullanılabilen yönetici seviyesindeki bir komut satırı yürütülebilir dosyasıdır. .wim, .vhd veya .vhdx biçimlerinde Windows görüntülerini bağlayabilir ve mevcut olarak yüklü Windows işletim sistemindeki sorunları gidermek için kullanılabilir.

 - /online
    Çevrimiçi bir görüntüyü değiştirdiğinizi belirtir (taramanın İnternet üzerinden çalıştırılacağını göstermez)
 - /cleanup-image
    Depolamayla ilgili sorunları giderebilecek daha kapsamlı bir denetimi tetikler
 - /checkhealth
    Depolamada bozulma algılanıp algılanmadığını görmek için temel denetim başlatır
 - /scanhealth
    Depolamayı bozulma açısından daha kapsamlı bir şekilde tarar
 - /restorehealth
    Depoyu bozulma açısından tarar ve bozulan dosyaları onarır

## `DISM /Online /Cleanup /CheckHealth`

Bu komut depolamada bozulma olup olmadığını anlamamız için temel bir denetim başlatır.
```
DISM /Online /Cleanup /CheckHealth
```

## `DISM /Online /Cleanup /ScanHealth`

Bu komut depolamayı bozulma açısından daha kapsamlı bir biçimde tarayıp sonuçları önümüze serer.
```
DISM /Online /Cleanup /ScanHealth
```

## `DISM /Online /Cleanup /RestoreHealth`

Bu komut bileşen deposunu bozulma açısından tarar ve bulduğu bozuk dosyaları onarır.
```
DISM /Online /Cleanup /RestoreHealth
```

## `tasklist`

Çalışan tüm task listleri getirir.
```
tasklist | findstr chrome
```

## `taskkill`

tasklist ile listelenen tasklardaki pin numaraları kullanılarak istenilen task sonlandırılır.
```
taskkill /f /pin 20184
```

## `netsh wlan show wlanreport`

Bu, sık kullandığınız Web tarayıcınızda açabileceğiniz bir HTML dosyası olarak kaydedilmiş bir kablosuz ağ raporu oluşturur. Rapor son üç günün tüm Wi-Fi olaylarını gösterir ve bu olayları Wi-Fi bağlantısı oturumlarına göre gruplandırır. Ayrıca, ağla ilgili birkaç komut satırı komut dosyasının sonuçlarını ve bilgisayarınızdaki tüm ağ bağdaştırıcılarının listesini gösterir.
```
netsh wlan show wlanreport
```

## `netsh interface show interface`

Kullanılan tüm interfaceleri görüntüler
```
netsh interface show interface
```

## `netsh interface ip show address | findstr “IP Address”`

İnterfacelerin aldığı tüm ip adreslerini gösterir.
```
netsh interface ip show address | findstr “IP Address
```

## `netsh interface ip show dnsservers`

interfacelerin kullandığı dns serverları gösterir
```
netsh interface ip show dnsservers
```

## `netsh advfirewall set allprofiles state off`

Windows'da kullanılan tüm firewall kurallarını kapatır
```
netsh advfirewall set allprofiles state off
```

## `netsh advfirewall set allprofiles state on`

Windows'da kullanılan tüm firewall kurallarını açar
```
netsh advfirewall set allprofiles state on
```

## `ping`

Belirli bir ip adresine yada dns'e  ping paketleri gönderir.
```
ping 192.168.1.1
```

## `ping -t`

Belirli bir ip adresine yada dns'e  sınırsız ping paketleri gönderir.
```
ping 192.168.1.1 -t
```

## `tracert`

Belirli bir ip adresine yada dns'e giden yolu bulur
```
tracert 192.168.1.1
```

## `tracert -d`

Belirli bir ip adresine yada dns'e dns adreslerini çözümlemeden gider. Hızlıdır.
```
tracert -d 192.168.1.1
```

### Netstat parametreleri
    -a	 Tüm TCP ve UDP bağlantıları ekrana basar.
    -e	 Gelen ve giden paket sayısının istatistiklerini görüntüler.
    -n	 Tüm bağlantıları rakamsal olarak görüntüler.
    -o	 Tüm bağlantıları PID numarası ve uygulama adına göre listeler.
    -p	 Bağlantıların kullandığı uygulama ve PID numaralarını ekrana basar.
    -s	 Kurallara göre istatistiksel verileri ekrana basar.
    -r	 IP yönlendirme tablosunun içeriğini görüntüler.

### Netstat çıktısında yer alan bağlantı durumlarının anlamları
    -ESTABLISHED	 Soket bağlantı gerçekleşmiş durumdadır.
    -SYN_SENT	 Soket bağlantı kurmaya çalışıyordur.
    -SYN_RECV	 Ağdan bir bağlantı isteği gelmiştir.
    -FIN_WAIT1	 Soket kapatılmış, bağlantı sonlandırılmak üzeredir.
    -FIN_WAIT2	 Bağlantı sonlandırılmıştır.Soket karşı ucun bağlantıyı sonlandırmasını beklemektedir.
    -TIME_WAIT	 Soket kapandıktan sonra gelebilecek paketleri alabilmek için beklemektedir.
    -CLOSED	 Soket kullanılmamaktadır.
    -CLOSE_WAIT	 Karşı uç bağlantıyı kapatmıştır.Soketin kapanması beklenmektedir.
    -LAST_ACK	 Karşı uç bağlantıyı sonlandırmış ve soketi kapatmıştır.Onay beklenmektedir.
    -LISTEN	 Soket gelebilecek bağlantılar için dinleme konumundadır.
    -CLOSING	 Yerel ve uzak soketler kapatılmış fakat tüm verilerini göndermemiş durumdadır.Tüm veriler gönderilmeden soketler kapanmaz.

## `route print`

Local routelarınızı listeler.
```
route print
```

## `route add`

Local route ekler
```
route add destination_network MASK subnet_mask  gateway_ip metric_cost
```
```
route add 192.168.35.0 MASK 255.255.255.0 192.168.0.2
```

## `route delete`

Eklenen routeleri siler
```
route delete destination_network
```

## `shutdown /r /fw /f /t 0`

Bilgisayarınızı yeniden başlatır açılışta biosa düşer.
```
shutdown /r /fw /f /t 0
```

## `shutdown /i	`

Uzaktan kapama-restart etme işlemleri için bir yardımcı arayüz açar
```
shutdown /i
```
