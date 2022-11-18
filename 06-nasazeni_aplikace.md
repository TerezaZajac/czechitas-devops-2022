Cíl: Nasadit aplikaci Netdata a zpřístupnit ji prostřednictvím reverzní HTTP proxy

Kroky:
1. Nainstalujte si aplikaci Netdata přes APT (balíček netdata)
2. Vytvořte pro aplikaci nový VirtualHost se jménem monitoring.local (po vzoru clinic.local)
• Tip: Budete potřebovat znát číslo portu, na kterém aplikace netdata poslouchá. Zkuste v
manuálnové stránce pro Netdata hledat klíčové slovo port, nebo koukněte do výstupu příkazu
sudo ss -ntlp – pozor, uvidíte tam porty dva, ale jen jeden z nich je pro webové rozhraní.

3. Nastavte si ve svých „hosts“ záznam 127.0.0.1 monitoring.local
4. Připojte se v prohlížeči na http://monitoring.local:8080. Měli byste vidět uživatelské rozhraní
aplikace Netdata.

![image info](/06/01.png)

![image info](/06/02.png)