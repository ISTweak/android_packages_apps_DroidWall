DroidWall
=======

【オリジナルとの違い】
------
/sbin/auがある場合は/sbin/auを利用するので、suコマンドを有効にする事なく実行出来ます。  
  
busyboxを  
/data/root/bin/busybox  
/data/root/busybox  
/data/local/bin/busybox  
app path/bin/busybox_g1  
  
grepを  
/data/root/bin/grep  
/data/local/bin/grep  
busybox grep  
  
iptablesを  
/data/root/bin/iptables  
/data/local/bin/iptables  
/system/bin/iptables2  
/system/bin/iptables  
app path/bin/iptables_armv5  
の順番で探して利用します。  
  
ルール適用のスクリプトを  
/data/data/com.googlecode.droidwall/app_bin/iptables.sh  
に書き出すように変更してあるので、他の操作をした時にスクリプトが上書きされません。  
init.rcやautoexec.shから直接実行することで、より早い段階でルールを有効にすることが出来ます。  


