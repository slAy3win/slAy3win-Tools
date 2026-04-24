@echo off
chcp 65001 >nul
title slAy3win PRO - Multitool v2.0
mode con: cols=125 lines=40
color 0c

:menu
cls
echo.
echo          ███████╗██╗      █████╗ ██╗   ██╗██████╗ ██╗    ██╗██╗███╗   ██╗
echo          ██╔════╝██║     ██╔══██╗╚██╗ ██╔╝╚════██╗██║    ██║██║████╗  ██║
echo          ███████╗██║     ███████║ ╚████╔╝  █████╔╝██║ █╗ ██║██║██╔██╗ ██║
echo          ╚════██║██║     ██╔══██║  ╚██╔╝   ╚═══██╗██║███╗██║██║██║╚██╗██║
echo          ███████║███████╗██║  ██║   ██║   ██████╔╝╚███╔███╔╝██║██║ ╚████║
echo          ╚══════╝╚══════╝╚═╝  ╚═╝   ╚═╝   ╚═════╝  ╚══╝╚══╝ ╚═╝╚═╝  ╚═══╝
echo.
echo   [+]═══════════════════════════════════[ MENU PRINCIPAL ]═══════════════════════════════════[+]
echo.
echo          [ Osint ]                        [ Security ]                     [ Discord ]
echo     [10] D0x Create                  [31] Proxy (Beta)                [60] Token Mass Dm
echo     [11] D0x Tracker                 [32] DDoS (Beta)                 [61] Token Delete Dm
echo     [12] Get Image Exif              [33] DDoS 2 (Beta)               [62] Status Changer
echo     [13] Google Dorking              [34] Web IP Info                 [63] Lang Changer
echo     [14] Username Osint              [35] Web Security                [64] House Changer
echo     [15] Email Tracker                                                [65] Theme Changer
echo     [16] Email Lookup                [ Osint 2 ]                      [66] Token Generator
echo     [17] Phone Number Lookup         [86] Username Osint 2            [67] Bot Server Nuker
echo     [18] Ip Lookup                   [87] Steam Osint                 [68] Bot Invite To ID
echo.                                     [88] TikTok Osint
echo                                      [89] Valorant Osint
echo   [+]═════════════════════════════════════════════════════════════════════════════════════════[+]
echo.
set /p choice="  slAy3win-PRO > "

:: --- LOGIQUE DE REDIRECTION ---
if "%choice%"=="10" goto d0x
if "%choice%"=="13" goto dorking
if "%choice%"=="14" goto user_osint
if "%choice%"=="18" goto ip_lookup
if "%choice%"=="31" goto proxy
if "%choice%"=="32" goto ddos
if "%choice%"=="60" goto token_action
if "%choice%"=="66" goto gen_token
if "%choice%"=="87" goto steam_osint
:: (Toutes les autres options non listées ici iront vers l'écran "En cours")
goto working

:d0x
cls
echo [!] CREATION DE DOSSIER D0X
set /p target="Nom de la cible : "
echo Dossier cree : %target%_D0X.txt
echo [Nom: %target%] > "%userprofile%\Desktop\%target%_D0X.txt"
pause
goto menu

:dorking
cls
echo [!] LANCEMENT GOOGLE DORKING
start https://www.google.com/search?q=filetype:txt+inurl:admin
pause
goto menu

:user_osint
cls
set /p user="Nom d'utilisateur : "
echo [!] Recherche Sherlock en cours...
start https://www.google.com/search?q=site:instagram.com+"%user%"+OR+site:twitter.com+"%user%"
pause
goto menu

:ip_lookup
cls
set /p ip="Adresse IP : "
curl https://ipapi.co/%ip%/json/
pause
goto menu

:proxy
cls
echo [!] RECUPERATION DE LISTE PROXY...
curl https://api.proxyscrape.com/v2/?request=displayproxies^&protocol=http^&timeout=10000^&country=all^&ssl=all^&anonymity=all
pause
goto menu

:ddos
cls
echo [!] SIMULATION ATTAQUE UDP...
echo Cible : %random%.%random%.%random%
timeout /t 1 >nul
echo Envoi de paquets 65500 bytes...
timeout /t 1 >nul
echo [OK] Attaque terminee.
pause
goto menu

:token_action
cls
echo [!] ERREUR CRITIQUE : TOKEN DISCORD NON DETECTE.
echo Veuillez inserer le token dans config.json
pause
goto menu

:gen_token
cls
echo [!] GENERATEUR DE TOKEN DISCORD (SIMULATION)
echo ODAy%random%Xz%random%Vv%random%
echo ODAz%random%Ab%random%Yy%random%
pause
goto menu

:steam_osint
cls
set /p steamid="ID Steam : "
start https://steamid.io/lookup/%steamid%
pause
goto menu

:working
cls
echo.
echo [!] L'OPTION
